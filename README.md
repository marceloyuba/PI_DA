

<p align='center'>
<img src ="scr\HenryLogo.jpg">
<p>


<p align='center'>
<h2 style="text-align: center; border: none;">
 Proyecto integrador de Data Analist
</h2>




 <h3 style="text-align: center; border: none;">
    Alumno Marcelo Yuba
</h3>

 <h2 align='center'>
 <b>Siniestros viales en la ciudad de Buenos Aires</b>
</h2>
<p align='center'>
<img src ="scr\Logotipo_de_la_Ciudad_de_Buenos_Aires.svg (1).png" height=100>
<p>
 <p style="text-align: left; border: none;">
<h3>
El Gobierno de la Ciudad Buenos Aires, genero una base de datos con las estadisticas de homicidios viales, mostrando Hechos y Victimas, nuestro trabajo es analizar estos datasets, hacer un ETL y un analisis EDA, para poder ver los datos de manera mas analitica, lo vamos a realizar en los <b>4 pasos más importantes del desarrollo<b>
</h3>
</p>
<h1>ETL</h1>
<p align='center'>
<img src ="scr\archivos.jpg">
<p>
<h3 style="text-align: left; border: none;">Se toma el archivo provisto, que se encuentra en formato Exel, pasamos a leerlo y hacer las transformaciones pertinentes como se ve en el archivo <a href="https://github.com/marceloyuba/PI_DA/blob/main/analisis/ETL.ipynb">ETL</a> que se encuentra en la carpeta <a href="https://github.com/marceloyuba/PI_DA/tree/main/analisis">analisis</a>
<br>
</h3>

<p>
<h3 style="text-align: left; border: none;">Conjuntamente al <a href="https://github.com/marceloyuba/PI_DA/blob/main/analisis/ETL.ipynb">ETL</a>, en Power Bi, se generaron transformaciones adicionales, debido a ser mas simple de implementar, como por ejemplo la normalizacion de los nombres de las calles y avenidas que originalmente se mostraban asi
<br>
</h3>
<p align='center'>
<img src ="scr\calles1.jpg" style="width: 30%;">
</p>

<p>
<h3 style="text-align: left; border: none;">Pasando a verse de esta manera</h3>
<br>
</p>

<p align='center'>
<img src ="scr\calles2.jpg">
</p>

<p>
<h3 style="text-align: left; border: none;">De esta manera las calles aparecen normalizadas en analisis posteriores en Power BI</h3>
<br>
</p>

<p>
<h2 style="text-align: left; border: none;">Dataset de comunas para geolocalizacion</h2>
<br>
</p>

<p>
<h3 style="text-align: left; border: none;">Se creo un nuevo Dataset poniendo los barrios pertenecientes a cada comuna, de esta manera, el mapa puede reconocer mas facilmente donde se encuentran ubicadas</h3>
<br>
</p>

<p align='center'>
<img src ="scr\comunas.jpg">
</p>

<p>
<h3 style="text-align: left; border: none;">Esta tabla se conecta a la columa COMUNA de la tabla de Hechos y asi se puden relacionar</h3>
<br>
</p>

<p align='center'>
<img src ="scr\conexion.jpg">
</p>

<p>
<h2 style="text-align: left; border: none;">Transformaciones de las tablas</h2>
<br>
</p>

<p>
<h3 style="text-align: left; border: none;">Tenemos la tabla de Hechos original</h3>
<br>
</p>
<p align='center'>
<img src ="scr\tablaHechosOriginal.jpg">
</p>
<p>
<h3 style="text-align: left; border: none;">Luego de un proceso de ETL en Power BI, terminamos dejando la tabla de esta manera</h3>
<br>
</p>
<p align='center'>
<img src ="scr\tablaHechosNew.jpg">
</p>
<p>