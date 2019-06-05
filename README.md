# Taller_2
Objetivo: Utilizar servicios disponibles en la nube para publicar mapas interactivos para la web.

# Publicación de cartografía vía web
Repositorio colaborativo para curso de publicación de cartografía vía web, Especialización en Geomática. 
## Investigadores:
#### Lorena Rayo Rocha `3101451`
#### Fernando Alcarcel Gutierrez `3101441`
#### Albeiro López Pulido `3101446`
---
# Precipitación media anual año 2012 Colombia

##xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
Cuál es el problema a tratar?
Por qué un mapa ayuda a resolverlo?
Descripción de los datos (tipos de geometrías, atributos, sistemas de referencia, urls para descarga de la información, etc)
Descripción del procesamiento realizado a los datos (ejm: transformaciones, filtros, geoprocesamiento, etc)
Descripción de los métodos / técnicas utilizadas para la visualización.
Se deben utilizar dos métodos diferentes para representar los datos.
Cada método debe presentarse en un mapa diferente
Descripción breve del procedimiento utilizado para publicar los mapas en la web
Ventajas / desventajas / dificultades de la publicación de mapas utilizando herramientas en la nube respecto al software desktop.
Urls públicos de los dos mapas interactivos
##xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx


## 1. Cuál es el problema a tratar?

Para determinar el personal necesario por departamento disponible para atender amenazas por deslizamientos en el año 2012, se requiere conocer la cantidad de lluvias anuales en cada departamento, sectorizado por cantidad de lluvias anuales y tomar esta información como insumo para conocer cual departamento necesita más inversión al respecto. 



## 2. Por qué un mapa ayuda a resolverlo?

La visualizacion de datos espaciales permite determinar el efecto que el aumento de una variable tiene sobre una zona, en este caso, departamentos de Colombia. 

Se consulta un **mapa de precipitación total anual** con el cual se pretende observar la precipitación media anual por departamento en Colombia en el año 2012 y con esto predecir zonas suceptibles a desastres naturales resultado de un aumento en las lluvias de una zona particular.

 ![alt text](MetodoNatualEqualInterv.png "Logo Title Text 1")

Mapa precipitación media anual del año 2012 para Colombia resaltando sus departamentos.

## 3. Descripción de los datos (tipos de geometrías, atributos, sistemas de referencia, urls para descarga de la información, etc)

Para la realización de este trabajo se tiene dos tipos de datos, un grupo de datos tipo polígono, los cuales describen zonas de igual valor de precipitación durante el año 2012 en Colombia, y otro grupo de datos tipo punto, el cual describe ciertas caracteristicas de las estaciones metereológicas como su fecha de instalación, su estado actual, su altura sobre el nivel del mar y su localización. los datos se tomaron de https://www.datos.gov.co/Ambiente-y-Desarrollo-Sostenible/Precipitaci-n-Media-Total-Anual-Promedio-Multianua/2bm3-399z 

Catalogo nacional de estaciones metereológicas: https://www.datos.gov.co/Ambiente-y-Desarrollo-Sostenible/Cat-logo-Nacional-de-Estaciones-del-IDEAM/hp9r-jxuu/data

## 4. Descripción del procesamiento realizado a los datos (ejm: transformaciones, filtros, geoprocesamiento, etc)

Para el desarrollo de este estudio se hicieron los siguiente procesos:

**Creación de archivo .shp:** Para el archivo de puntos se tomaron los datos crudos en tabla de excel y con la ayuda del software ArcMap se convirtieron a formato .shp de tipología de punto con todos sus atributos. 


**Descarga del archivo .shp:** Los poligonos utilizados en el estudio se descargaron directamente en formato .shp y se cargaron de forma fácil en la herramienta Carto. 


## 5. Descripción de los métodos / técnicas utilizadas para la visualización.

Para la visualización de los datos se seleccionó la herramienta [Carto](https://carto.com/) con la cual es posible no solo cargar los datos adquiridos, sino analizarlos de diferente forma con diferentes herramientas para obtener más información de la que por si tienen en sus atributos. Inicialmente se realizo un cambio de estilo al mapa, utilizando una coloración de acuerdo a su valor, lo cual permite tener una idea clara de las zonas con mayor o menor precipitaciones anuales. a dicha capa de poligonos se le relaciona una leyenda y una herramienta de selección para cada cantidad de precipitación. 

Descripción breve del procedimiento utilizado para publicar los mapas en la web

https://geoportal.igac.gov.co/es/contenido/datos-abiertos-catastro

Mapa estaciones en cada departamento: https://geomaticos.carto.com/builder/ba2b705a-2b36-4ff2-97d5-49de0a03bb12/embed


<style>.embed-container {position: relative; padding-bottom: 80%; height: 0; max-width: 100%;} .embed-container iframe, .embed-container object, .embed-container iframe{position: absolute; top: 0; left: 0; width: 100%; height: 100%;} small{position: absolute; z-index: 40; bottom: 0; margin-bottom: -15px;}</style><div class="embed-container"><iframe width="500" height="400" frameborder="0" scrolling="no" marginheight="0" marginwidth="0" title="Estaciones" src="//unimilitar.maps.arcgis.com/apps/Embed/index.html?webmap=8c5ab5af7e164052bbef57fe6598ff8c&extent=-87.5583,-1.9194,-60.9054,10.1772&zoom=true&previewImage=false&scale=true&disable_scroll=true&theme=light"></iframe></div>


Información utilizada: 

| Nombre        | Tipo           | Extensión  |
| ------------- |:-------------:| -----:|
|Precipitación     | Polígono | .shp |
| Estaciones     | Punto      |   .shp |

## 6.Ventajas/ desventajas/ dificultades/ diferencias encontradas al utilizar qgis y arcgis para el desarrollo del ejercicio.

`Según las instrucciones del cliente, el trabajo fue realizado unicamente en el software Arc Gis. `

