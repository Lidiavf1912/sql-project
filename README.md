# sql-project

![](https://github.com/Lidiavf1912/sql-project/blob/main/imagenes/imagen%20cabecera%20readme.jpg)

## Indice:
1.[Contexto](#Contexto)\
2.[As Is](#As-Is)\
3.[To Be](#To-Be)\
4.[Desarrollo del proyecto](#Desarrollo_del_proyecto)\
5.[Conclusiones y sugerencias](#Conclusiones_y_sugerencias)

## 1. Contexto <a name="Contexto"/>
En este proyecto, desplegaremos una labor de consultoría para un videoclub que opera en dos ubicaciones distintas. Los únicos datos disponibles para este videoclub se encuentran en siete hojas de cálculo de Excel, que incluyen información sobre actores, categorías de películas, películas en stock, idiomas, antiguos discos duros, alquileres y más. Estos documentos contienen detalles sobre las películas disponibles, tiendas de la empresa, características de las películas (actores, idiomas, comentarios, etc.), y los identificadores de los empleados, entre otros datos.

## 2. As is <a name="As-Is"/>
En el funcionamiento diario de la empresa, los clientes suelen preguntar sobre las películas disponibles en las tiendas, las películas en las que actúan ciertos actores, y otros detalles relacionados. Desafortunadamente, los empleados no tienen los conocimientos técnicos necesarios para realizar consultas en las hojas de Excel y proporcionar respuestas a estas preguntas.

## 3. To be <a name="To-Be"/>
Para abordar esta problemática, desarrollaremos una base de datos en MySQL para almacenar y relacionar la información contenida en las hojas de Excel. Además, dado que los empleados carecen de conocimientos de programación, crearemos un panel de control en Tableau que les permitirá consultar la información solicitada por los clientes de manera rápida y sencilla.

## 4. Desarrollo del proyecto <a name="Desarrollo_del_proyecto"/>

### 4.1 Limpieza de datos
Para comenzar, hemos realizado una limpieza de los archivos CSV proporcionados por la empresa para garantizar la precisión de los datos. Hemos convertido todos los nombres a minúsculas, eliminado actores duplicados y columnas irrelevantes, y hemos agregado nuevas columnas para describir las características de las películas, como la disponibilidad de tráilers, comentarios, escenas eliminadas e imágenes detrás de escena. Posteriormente, exportamos estos archivos CSV depurados.
Para acceder al documento pulse [aqui](https://github.com/Lidiavf1912/sql-project/blob/main/python/limpieza%20csvs.ipynb).

### 4.2 Creación de una base de datos
Una vez que contamos con los archivos limpios, los hemos importado a MySQL y hemos establecido relaciones entre ellos para permitir consultas con datos de todos los archivos CSV. Finalmente, hemos creado una vista que incluye los nombres y apellidos de los actores, el título de las películas y las ubicaciones de las tiendas de la empresa.
Las queries utilizadas para realizar el esquema de la bbdd se disponen [aqui](https://github.com/Lidiavf1912/sql-project/blob/main/mysql/esquema%20y%20relaciones%20bbdd.txt).
La query realizada para crear la vista en la base da datos aparece [aqui](https://github.com/Lidiavf1912/sql-project/blob/main/mysql/query%20vista%20bbdd.txt).

### 4.3 Realización del dashboard
Para concluir, hemos cargado la vista que creamos en la base de datos para desarrollar un panel de control en Tableau. Hemos realizado un dashboard que permitirá a los empleados consultar la información de manera sencilla y con la posibilidad de interactuar mediante filtros. En este dashboard hemos incorporación información sobre los nombres de las películas que dispone la empresa, las tiendas en las que están disponibles y los actores que aparecen en estas.
Link al dashboard [aqui](https://public.tableau.com/app/profile/lidia.vi.uales/viz/stockdepeliculasvideoclub/Dashboard1?publish=yes)

## 5. Conclusiones y sugerencias <a name="Conclusiones_y_sugerencias"/>
Finalmente, hemos logrado mejorar la experiencia del usuario al poder resolver las consultas de los clientes los empleados.
Por otra parte, hemos identificado que la empresa carece de una página web. Por lo tanto, nuestro equipo de desarrollo web puede crear un sitio web que ofrezca acceso al panel de control desarrollado. Esto permitirá a los clientes consultar la información en línea desde cualquier ubicación, sin necesidad de acudir a la tienda física y consultar al personal para resolver sus dudas. Además, se pueden recopilar otras dudas comunes que realicen los clientes para realizar más dashboards que ayuden a la experiencia del usuario.






