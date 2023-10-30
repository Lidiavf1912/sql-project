# sql-project

![](https://github.com/Lidiavf1912/sql-project/blob/main/imagenes/imagen%20cabecera%20readme.jpg)

## Contexto

En este proyecto, desplegaremos una labor de consultoría para un videoclub que opera en dos ubicaciones distintas. Los únicos datos disponibles para este videoclub se encuentran en siete hojas de cálculo de Excel, que incluyen información sobre actores, categorías de películas, películas en stock, idiomas, antiguos discos duros, alquileres y más. Estos documentos contienen detalles sobre las películas disponibles, tiendas de la empresa, características de las películas (actores, idiomas, comentarios, etc.), y los identificadores de los empleados, entre otros datos.

## 1.1 As is
En el funcionamiento diario de la empresa, los clientes suelen preguntar sobre las películas disponibles en las tiendas, las películas en las que actúan ciertos actores, y otros detalles relacionados. Desafortunadamente, los empleados no tienen los conocimientos técnicos necesarios para realizar consultas en las hojas de Excel y proporcionar respuestas a estas preguntas.

## 1.2 To be
Para abordar esta problemática, desarrollaremos una base de datos en MySQL para almacenar y relacionar la información contenida en las hojas de Excel. Además, dado que los empleados carecen de conocimientos de programación, crearemos un panel de control en Tableau que les permitirá consultar la información solicitada por los clientes de manera rápida y sencilla.

## Limpieza de datos
Para comenzar, hemos realizado una limpieza de los archivos CSV proporcionados por la empresa para garantizar la precisión de los datos. Hemos convertido todos los nombres a minúsculas, eliminado actores duplicados y columnas irrelevantes, y hemos agregado nuevas columnas para describir las características de las películas, como la disponibilidad de tráilers, comentarios, escenas eliminadas e imágenes detrás de escena. Posteriormente, exportamos estos archivos CSV depurados.
Se puede consultar el proceso realizado en el archivo 'limpieza csvs' en la carpeta 'python.

## Realización de bbdd
Una vez que contamos con los archivos limpios, los hemos importado a MySQL y hemos establecido relaciones entre ellos para permitir consultas con datos de todos los archivos CSV. Finalmente, hemos creado una vista que incluye los nombres y apellidos de los actores, el título de las películas y las ubicaciones de las tiendas de la empresa.
Las queries realizadas para este apartado se dispone dentro de la carpeta mysql.

## Dashboard de Tableau
Para concluir, hemos cargado la vista que creamos en la base de datos para desarrollar un panel de control en Tableau. Esto permitirá a los empleados y clientes consultar la información de manera sencilla y con la posibilidad de interactuar mediante filtros.
Link al dashboard: https://public.tableau.com/app/profile/lidia.vi.uales/viz/stockdepeliculasvideoclub/Dashboard1?publish=yes


## Sugerencias
Hemos identificado que la empresa carece de una página web. Por lo tanto, nuestro equipo de desarrollo web puede crear un sitio web que ofrezca acceso al panel de control desarrollado. Esto permitirá a los clientes consultar la información en línea desde cualquier ubicación, sin necesidad de acudir a la tienda física y consultar al personal para resolver sus dudas.






