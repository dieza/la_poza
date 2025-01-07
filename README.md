# la_poza
Roman castra
En este repositorio puedes encontrar los enlaces necesarios para localizar y visibilizar el campamento romano de La Poza (Campóo de Enmedio, Cantabria). Como
Lo primero que necesitamos son los ficheros LiDAR del lugar que se pueden descargar desde los siguientes enlaces: 

https://centrodedescargas.cnig.es/CentroDescargas/detalleArchivo?sec=11731130
https://centrodedescargas.cnig.es/CentroDescargas/detalleArchivo?sec=11731201
https://centrodedescargas.cnig.es/CentroDescargas/detalleArchivo?sec=11731129
https://centrodedescargas.cnig.es/CentroDescargas/detalleArchivo?sec=11731200

Ahora necesitamos instalar en el ordenador el programa CloudCompare (https://www.cloudcompare.org)

El proceso es relativamente sencillo.
1. Arrancamos CloudCompare
2. Arrastramos los ficheros que nos hemos descargado
3. Hacemos un 'Edit-->Merge' -unimos- con todos los fichertos
4. Escogemos 'Scalar Field'
5. Escogemos 'Classification'
6. Filtramos los datos que nos interesan, el valor 2 (=suelo) con  'Edit-->Scalar Fields-->Filter by value'
7. Selecciónamos la opción 'export'
8. Selecciónamos la capa exportada y vamos al menú 'Tools-->Projection-->rasterize'
9. Escogemos las zetas (z), en el step ponemos 0.25 y decimos que nos rellene las celdas vacías ('empty cells') con un valor interpolado ('interpolate')
10. Exportamos el resultado (heights) como raster y lo llamamos 'La_Poza_lidar3_mdt.tif'
Ahora nos vamos a Qgis y cargamos ese fichero en una vista epsg 25830
11. En caso de no tenerlo instalado, instalamos el plugin Relief Visualization Tool
12. Lo aplicamos a nuestro fichero
