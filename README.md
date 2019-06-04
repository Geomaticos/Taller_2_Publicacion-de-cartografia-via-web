# Taller_2
Taller_2

# Publicación de cartografía vía web
Repositorio colaborativo para curso de publicación de cartografía vía web, Especialización en Geomática. 
## Investigadores:
#### Lorena Rayo Rocha `3101451`
#### Fernando Alcarcel Gutierrez `3101441`
#### Albeiro López Pulido `3101446`
---
# Precipitación media anual año 2012 Colombia

## 1. Cuál es el problema a tratar?

Para determinar el personal necesario por departamento disponible para atender amenazas por deslizamientos en el año 2012, se requiere conocer la cantidad de lluvias anuales en cada departamento, sectorizado por cantidad de lluvias anuales y tomar esta información como insumo para conocer cual departamento necesita más inversión al respecto. 



## 2. Por qué un mapa ayuda a resolverlo?

La visualizacion de datos espaciales permite determinar el efecto que el aumento de una variable tiene sobre una zona, en este caso, departamentos de Colombia. 

Se consulta un **mapa de precipitación total anual** con el cual se pretende observar la precipitación media anual por departamento en Colombia en el año 2012 y con esto predecir zonas suceptibles a desastres naturales resultado de un aumento en las lluvias de una zona particular.

 ![alt text](MetodoNatualEqualInterv.png "Logo Title Text 1")

Mapa precipitación media anual del año 2012 para Colombia resaltando sus departamentos.

## 3. Descripción del mapa temático (variable semleccionada, utilidad?

Para la realización del trabajo se seleccionó la variable de precipitación anual medida en mm por año, la cual se obtiene con un Pluviómetro manual lo cual es un indicador simple de la lluvia caída, consiste en un recipiente especial cilíndrico, por lo general de plástico, con una escala graduada en donde todas las marcas están a igual distancia entre sí. La altura del agua que llena la jarra es equivalente a la precipitación y se mide en mm. 

## 4. Descripción de los métodos de clasificación seleccionados. Cuál es mejor para la variable seleccionada? por qué?

Se utilizaron dos metodos de clasificación: "Natural Breaks" y "Equal Interval". Los dos métodos los describimos a continuación:

**Natual Breaks:** Las clases de cortes naturales se basan en las agrupaciones naturales inherentes a los datos. Los cortes de clase se caracterizan porque agrupan mejor los valores similares y maximizan las diferencias entre clases. Por tanto son los más adecuados para la clase de datos que tenemos.

[Mapa Precipitación media anual año 2012 mediante clasificación Natural Breaks](https://raw.githubusercontent.com/Geomaticos/Publicacion-de-cartografia-via-web/master/MetodoNatualBreaks8%20clases.png)

**Equal Interval:** Los intervalos equivalentes dividen el rango de valores de atributo en subrangos de igual tamaño. Con ello se permite especificar el número de intervalos. Este tipo de clasificaciones no es recomendado cuando se grafican datos que no guardan una distribucion sistemática, como el caso de cualquier evento natural. 

[Mapa Precipitación media anual año 2012 mediante clasificación Equal Interval](https://raw.githubusercontent.com/Geomaticos/Publicacion-de-cartografia-via-web/master/MetodoNatualEqualInterv.png)


## 5. Listado de fuentes de datos seleccionados( proveedor, enlace para descarga, descripcón, procedimiento utilizado(plugins extensiones, procesos, transformaciones de datos, etc)

Se descargó la informacion correspondiente a precipitación media anual de la pagina de [Sistema de información ambiental de Colombia](http://www.siac.gov.co/catalogo-de-mapas) con la cual se puede graficar los poligonos de precipitación media anual. Este mapa nos describe zonas con igual cantidad de precipitacion anual en Colombia en el año 2012, por otra parte descargamos de la pagina https://sites.google.com/site/seriescol/shapes el shape con la informacion de departamentos los cuales pueden ser superpuestos con el para obtener los datos solicitados por los organismos de emergencia. 

Información utilizada: 

| Nombre        | Tipo           | Extensión  |
| ------------- |:-------------:| -----:|
|Precipitación     | Polígono | .shp |
| Departamentos     | Polígono      |   .shp |

## 6.Ventajas/ desventajas/ dificultades/ diferencias encontradas al utilizar qgis y arcgis para el desarrollo del ejercicio.

`Según las instrucciones del cliente, el trabajo fue realizado unicamente en el software Arc Gis. `

