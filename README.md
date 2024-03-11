<p align='center'>
<img src ="scr\HenryLogo.jpg">
<p>


<p align='center'>
<h2 align='center'>
 Proyecto integrador de Data Analist
</h2>
</p>


<p>
 <h3 align='center'>
    Alumno Marcelo Yuba
</h3>
</p>

<p>
 <h2 align='center'>
 <b>Siniestros viales en la ciudad de Buenos Aires</b>
</h2>
</p>
<br>

<h1>Glosario del README</h1>
<h3>Secciones de este documento</h3>
<h3><a href="#intro">Introduccion</a></h3>
[Ir a la ETL](#ETL)<br>
[EDA](#EDA)
<h3><a href="#Hipotesis">Hipotesis</a></h3>
<h3><a href="#Conclusiones">Conclusiones</a></h3>
<h1></h1>
</p>
<br>

<p align='center'>
<img src ="scr\Logotipo_de_la_Ciudad_de_Buenos_Aires.svg (1).png" height=100>
<p>
 <p style="text-align: left; border: none;">
 <h1 id="intro">Rol a desarrollar</h1>
<h3>
El Observatorio de Movilidad y Seguridad Vial (OMSV), centro de estudios que se encuentra bajo la órbita de la Secretaría de Transporte del Gobierno de la Ciudad Autónoma de Buenos Aires, nos solicita la elaboración de un proyecto de anális de datos, con el fin de generar información que le permita a las autoridades locales tomar medidas para disminuir la cantidad de víctimas fatales de los siniestros viales. Para ello, nos disponibilizan un dataset sobre homicidios en siniestros viales acaecidos en la Ciudad de Buenos Aires durante el periodo 2016-2021. Este dataset se encuentra en formato xlsx y contiene :<b> hechos y víctimas </b>. Asimismo, observarán que incluye otras dos hojas adicionales de diccionarios de datos, que les podrá servir de guía para un mayor entendimiento de la data compartida.
</h3>
<br>

<p align='center'>
<img src ="scr\camino.jpg">
<p>
<br>

<p align='center' {#ETL}>
<img src ="scr\barraETL.jpg">
<p>
<br>

<p align='center'>
<img src ="scr\archivos.jpg">
<img src ="scr\etl.jpg">

<p>
<h3 style="text-align: left; border: none;">Se toma el archivo provisto, que se encuentra en formato Exel, pasamos a leerlo y hacer las transformaciones pertinentes como se ve en el archivo <a href="https://github.com/marceloyuba/PI_DA/blob/main/analisis/ETL.ipynb">ETL</a> que se encuentra en la carpeta <a href="https://github.com/marceloyuba/PI_DA/tree/main/analisis">analisis</a>
<br>
</h3>
</p>

<p>
<h3 style="text-align: left; border: none;">Conjuntamente al <a href="https://github.com/marceloyuba/PI_DA/blob/main/analisis/ETL.ipynb">ETL</a>, en Power Bi, se generaron transformaciones adicionales, debido a ser mas simple de implementar, como por ejemplo la normalizacion de los nombres de las calles y avenidas que originalmente se mostraban asi
<br>
</h3>

<p align='center'>
<img src ="scr\calles1.jpg">
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
<h3 style="text-align: left; border: none;">Tenemos la tabla de Victimas original</h3>
<br>
</p>

<p align='center'>
<img src ="scr\tablaVictimasOriginal.jpg">
</p>

<p>
<h3 style="text-align: left; border: none;">Luego de un proceso de ETL en Power BI, terminamos dejando la tabla de esta manera</h3>
<br>

</p>
<p align='center'>
<img src ="scr\tablaVictimasNew.jpg">
</p>

<p>
<h2 style="text-align: left; border: none;">Con esto pasamos a analizar en Power BI y hacer los graficos e interacciones para presentar el proyecto</h2>
<br>
</p>
<br>

<p align='center' id="EDA">
<img src ="scr\barraEDA.jpg">
<p>
<br>

<p align='center'>
<img src ="scr\eda.jpg">
<p>
<br>

<p>
<h3 style="text-align: left; border: none;">Una vez concluido el ETL, pasamos a realizar el <a href="https://github.com/marceloyuba/PI_DA/blob/main/analisis/EDA.ipynb">EDA</a> que se encuentra en la carpeta <a href="https://github.com/marceloyuba/PI_DA/tree/main/analisis">analisis</a>, en el mismo, vamos a hacer un analisis de las variables mas significativas y graficar los datos a ver que resultados brindan
<br>


<h1>Variables a ser analizadas: </h1>

* Tabla de Hechos:
    * Año
    * Mes
    * Franja Horaria
    * Victima
    * Comuna
    * Acusado
    * Tipo de Via    

<h3> Despues de ver los datos, se consideraron esta variables por ser las que generan mejores resultados a la hora de graficarlos, mostramos un ejemplo a continuacion:</h3>
<br>

<p align='center'>
<img src ="scr\grafico1.png">
<p>
<br>

<h3>En este podemos ver como la mayor cantidad de victimas son las motos, a continuacion veremos las conclusiones que sacamos del EDA</h3>



<h1 id="Hipotesis">Hipotesis</h1>

