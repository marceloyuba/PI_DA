<p align='center'>
<img src ="scr\HenryLogo.jpg">
<p>


<p align='center'>
<h2 align='center'>
 Proyecto integrador de Data Analyst
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

<p align='center'>
<img src ="scr\Logotipo_de_la_Ciudad_de_Buenos_Aires.svg (1).png" height=100>
</p>
<h1>Glosario del README</h1>

* Indice
    * Introduccion
    * ETL
    * EDA
    * Hipotesis y  Conclusiones

<br>

<p align='center' {#ETL}>
<img src ="scr\barraROL.jpg">
<p>
<h1></h1>
<h3>
El Observatorio de Movilidad y Seguridad Vial (OMSV), centro de estudios que se encuentra bajo la órbita de la Secretaría de Transporte del Gobierno de la Ciudad Autónoma de Buenos Aires, nos solicita la elaboración de un proyecto de anális de datos, con el fin de generar información que le permita a las autoridades locales tomar medidas para disminuir la cantidad de víctimas fatales de los siniestros viales. Para ello, nos disponibilizan un dataset sobre homicidios en siniestros viales acaecidos en la Ciudad de Buenos Aires durante el periodo 2016-2021. Este dataset se encuentra en formato xlsx y contiene :<b> hechos y víctimas </b>. Asimismo, observarán que incluye otras dos hojas adicionales de diccionarios de datos, que les podrá servir de guía para un mayor entendimiento de la data compartida.
</h3>
<br>

<p align='center'>
<img src ="scr\camino.jpg">
<p>
<br>

 <h1>Tecnologias</h1>

* Las tecnologias usadas en este proyecto son:
  * Pandas
  * Numpy
  * Matplotlib
  * Seaborn
  * Power BI
<h3></h3>
<br>

<p align='center' {#ETL}>
<img src ="scr\barraETL.jpg">
<p>

<h1></h1>
<p align='center'>
<img src ="scr\archivos.jpg">
<img src ="scr\etl.jpg">

<p>
<h3 style="text-align: left; border: none;">Se toma el archivo provisto, que se encuentra en formato Excel, pasamos a leerlo y hacer las transformaciones pertinentes como se ve en el archivo <a href="https://github.com/marceloyuba/PI_DA/blob/main/analisis/ETL.ipynb">ETL</a> que se encuentra en la carpeta <a href="https://github.com/marceloyuba/PI_DA/tree/main/analisis">analisis</a>
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

<h3>En este podemos ver como la mayor cantidad de victimas son las motos, a continuacion veremos las hipotesis y conclusiones que sacamos del EDA y Power BI</h3>

<br>
<p align='center' {#ETL}>
<img src ="scr\barraHIpo.jpg">
<p>
<h1></h1>


<h3>Habiendo realizado el EDA, nos permite anticipar los resultados para un posterior analisis en Power BI, de esta manera llegamos a las siguientes hipotesis y posteriores concluciones</h3>

<h2>Ultimo tremestre 2021</h2>

<h3>1. Analizar con un KPI, si los accidentes viales bajaron un 10% respecto al ultimo semestre de 2021, en caso de ser negativo, plantear soluciones para reducir los siniestros</h3>
<br>

<p align='center'>
<img src ="scr\analisis\KPI10.jpg">
<p>

<br>
<h3>Como se ve en el KPI, no logramos alcanzar la reduccion que planteamos, debido que fue 2021 donde recien se volvia a activar de a poco la actividad comercial y de libre circulacion luego de la cuerentena por el COVID 19, la tasa de accidentes es mucha, de todas formas, hay que hacer una capacitacion vial a los conductores, sobre todo de motos, que siempre registran la mayor cantidad de siniestros, la mayoria son repartidores de aplicaciones como Pedidos Ya y otra parte hace cadeteria, ya sea de oficina como Mercado Libre, la que desde 2020 crecio exponencialmente gracias a la cuarentena. Por ultimo reforzar los controles de inspectores de transito para que se vea el estado en que manejan(con o sin casco, alcoholizados, vehiculo en condiciones) </h3>
<br>

<h3>2. Son los Adultos Mayores, propensos a accidentes viales y en que cirscunstancia suceden estos siniestros, tomamos la edad jubilatoria que en caso de las mujeres es 60 años y hombres 65 años, nuestra medida seran los 60 años. </h3>
<br>
<p align='center'>
<img src ="scr\analisis\EtarioUltimo.jpg">
<p>
<br>

<h3>Los resultados que arroja son interesantes, nos muestra que la mayoria, medianamente acorde a su edad, son siniestros ocurridos en avenidas y siendo peatones en su mayoria, como conductores de auto y bicicleta en menor medida, pero tambien tomemos en cuenta que en epocas de cuarentena, la mayoria de las personas salian caminando a supermercados y locales de su propia zona, debido a la restriccion que se encontraba vigente.<br> La mayor cantidad junta de accidentes es la Comuna 1, como casi en todo los analisis, puede deberse que el cruce de la avenida 9 de julio es complicado debido al ancho de esta, personas con movilidad mas reducida encuentran complicado el cruce a tiempo, y en otros, cruzar por lugares fuera de las sendas peatonales. Una solucion posible, es en los puntos mas neuralgicos, poner puentes peatonales</h3>
<br>

<h3>3. En contraste con la anterior, son los jovenes propensos a accidentes viales y en que cirscuntancia suceden, tomaremos la mayoria de edad que es 18 años hasta los 25 años, sabiendo que los planes de medicina toman estas edades como juventud </h3>
<br>

<p align='center'>
<img src ="scr\analisis\EtarioUltimo18.jpg">
<p>
<br>

<h3>En este caso como el anterior, vemos que la mayor incidencia es en conductores de moto, esto debido en su mayoria a jovenes que buscan una forma de hacer dinero sin experiencia laboral y la mayoria la tiene como un medio economico de transporte, o, de bajo costo para poder empezar trabajando para aplicaciones de comida o mensajeria.
<br>
Se podrian brindar cursos de manejo responsable en moto, ya que a la fecha, no existen
</h3>
<br>

<h3>4. Cual es la Comuna con mayor cantidad de accidentes y tratar de analizar el porque de este fenomeno</h3>

<br>
<p align='center'>
<img src ="scr\analisis\comuna.jpg">
<p>
<br>

<h3>Como podemos ver, la Comuna 1, en este caso como en muchos otros, es la comuna con mas siniestros, esto debido a que parte de la ciudad ocupa, Como se puede observar la mayoria de los siniestros son peatones, bicicletas y motos. La gran cantidad de trafico automotor genera estos accidentes. </h3>

<br>
<p align='center'>
<img src ="scr\analisis\mapaComuna.jpg">
<p>
<br>

<h3>Basicamente ocupa la parte centrica de la ciudad, avenidas como, Corrientes, 9 de julio( comprende las calles laterales que se llaman Cerrito/Lima y Carlos Pellegrini/ Bernardo de Irigoyen, Avenida Corrientes hace el cambio de nombre ), Avenida de Mayo, Belgrano, Cordoba y Santa Fe, las cuales son muy concurridas por sus oficinas y locales, hacen de esta un caos de trafico mas aun en las horas pico y de corrida bancaria y de mercado.
<br>
Una solucion probada para este problema es la obligacion de circular por menos partes, reducir los espacios de estacionamiento y el ancho de las calles, aunque sin una medida que obligue la menor circulacion de vehiculos, generan mas embotellamientos.
<br>
Implementar la limitacion de circulacion por letra de patente, cobrar un cargo de congestion (como se hace en Londres), valores altos de peaje en horas pico a vehiculos con menos de dos ocupantes para el ingreso a un perimetro especifico, reduciria sustancialmente el trafico en la Comuna 1, haciendo un perimetro entre, Av. Pueyrredon, Av. San Juan, Av. Libertador y Av. Alicia Morau de Justo (Puerto Madero).
</h3>

<br>
<p align='center'>
<img src ="scr\analisis\mapaBloque.jpg">
<p>
<br>

<h3>5. Cual es el mayor causante de siniestros  y en que comuna son la mayor cantidad y quienes son los mas siniestrados y donde</h3>

<br>
<p align='center'>
<img src ="scr\analisis\5utlimoTrimestre.jpg">
<p>
<br>

<h3>Tomando en cuenta el analisis previo en el EDA.</h3>

<br>
<p align='center'>
<img src ="scr\analisis\acusados.jpg">
<p>
<br>

<h3>Se hizo un analisis al respecto en Power BI buscando al Auto como el mayor causante de accidentes, y en el analisis por ultimo semestre concuerda con lo visto. Las medidas mencionadas en el punto anterior, aplican de igual manera para esta conclusion </h3>