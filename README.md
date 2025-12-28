# la_poza
Roman castra
En este repositorio puedes encontrar los enlaces necesarios para localizar y visibilizar el campamento romano de La Poza (Campóo de Enmedio, Cantabria). Como
Lo primero que necesitamos son los ficheros LiDAR del lugar que se pueden descargar desde los siguientes enlaces: 

https://centrodedescargas.cnig.es/CentroDescargas/detalleArchivo?sec=11731130
https://centrodedescargas.cnig.es/CentroDescargas/detalleArchivo?sec=11731201
https://centrodedescargas.cnig.es/CentroDescargas/detalleArchivo?sec=11731129
https://centrodedescargas.cnig.es/CentroDescargas/detalleArchivo?sec=11731200

Los enlaces han dejado de funcionar los ficheros se pueden descargar desde la carpeta datos.


[PNOA_2023_CANT_407-4757_NPC01.laz](datos/PNOA_2023_CANT_407-4757_NPC01.laz)
[PNOA_2023_CANT_408-4757_NPC01.laz](datos/PNOA_2023_CANT_408-4757_NPC01.laz)
[PNOA_2023_CANT_407-4758_NPC01.laz](datos/PNOA_2023_CANT_407-4758_NPC01.laz)
[PNOA_2023_CANT_408-4758_NPC01.laz](datos/PNOA_2023_CANT_408-4758_NPC01.laz)

Ahora necesitamos instalar en el ordenador el programa CloudCompare (https://www.cloudcompare.org)

El proceso es relativamente sencillo.
1. Arrancamos CloudCompare
2. Arrastramos los ficheros que nos hemos descargado
3. Hacemos un 'Edit-->Merge' -unimos- con todos los ficheros ![alt text](https://github.com/dieza/la_poza/blob/main/merge.png?raw=true)
4. Escogemos 'Scalar Field' ![alt text](https://github.com/dieza/la_poza/blob/main/scalar.png?raw=true)
5. Escogemos 'Classification'
6. Filtramos los datos que nos interesan, el valor 2 (=suelo) con  'Edit-->Scalar Fields-->Filter by value' ![alt text](https://github.com/dieza/la_poza/blob/main/filtro.png?raw=true)
7. Selecciónamos la opción 'export' ![alt text](https://github.com/dieza/la_poza/blob/main/export.png?raw=true)
8. Selecciónamos la capa exportada y vamos al menú 'Tools-->Projection-->rasterize' ![alt text](https://github.com/dieza/la_poza/blob/main/rasterize.png?raw=true)
9. Escogemos las zetas (z), en el step ponemos 0.25 y decimos que nos rellene las celdas vacías ('empty cells') con un valor interpolado ('interpolate') ![alt text](https://github.com/dieza/la_poza/blob/main/interpolar.png?raw=true)
10. Exportamos el resultado (heights) como raster y lo llamamos 'La_Poza_lidar3_mdt.tif' ![alt text](https://github.com/dieza/la_poza/blob/main/mdt.png?raw=true) ![alt text](https://github.com/dieza/la_poza/blob/main/mdt2.png?raw=true)
Ahora nos vamos a Qgis y cargamos ese fichero en una vista epsg 25830
11. En caso de no tenerlo instalado, instalamos el plugin Relief Visualization Tool ![alt text](https://github.com/dieza/la_poza/blob/main/rvt.png?raw=true)
12. Lo aplicamos a nuestro fichero ![alt text](https://github.com/dieza/la_poza/blob/main/rvt2.png?raw=true)
13. Vemos el resultado:
    ![alt text](https://github.com/dieza/la_poza/blob/main/la_poza.jpg?raw=true)
    Si quieres saber más de los campamentos romanos de la poza (https://dialnet.unirioja.es/servlet/articulo?codigo=2214250)
