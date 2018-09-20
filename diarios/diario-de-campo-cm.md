# Diario de campo

## 05-08-18

### Nomenclatura y árbol de navegación

Encuentro algunas dificultades para nombrar los archivos. Hay 3 elementos importantes: 

* Sección de la tutela
  * Hechos
  * Pretensiones
  * Consideraciones
  * Decisiones
* Año de la tutela
* Consecutivo
* Clasificador único: n.° de radicación

Podría ser en ese orden, p. ej.: "hechos-0001-2010.txt"

¿Funcionaría esa nomenclatura si no todas las tutelas tienen el mismo # de partes?

Árbol de navegación

* corpus-tutelas
  * sección
    * año

## 06-08-18

### Experimentación con Mallet (Windows)

* En la creación del archivo .mallet es necesario usar el comando stoplist-file stoplists\es.txt para que el programa cargue la lista de palabras vacías en español. De otro modo, tomará una lista por defecto de Java. Comando completo para cargar los archivos con la lista en español:

  ```
  bin\mallet import-dir --input mydata --output prueba2.mallet --keep-sequence --remove-stopwords --stoplist-file stoplists\es.txt
  ```

* C[odigo para sacar primera lista de tópicos: 

  ```
  bin\mallet train-topics  --input NOMBRE DEL ARCHIVO.mallet
  ```

* Código para correr el modelo de tópicos. Cambiar los parámetros de n.° de tópicos según sea necesario. 

  ```
  bin\mallet train-topics  --input tutorial.mallet  --num-topics 20 --optimize-interval 20 --output-state topic-state.gz  --output-topic-keys tutorial_keys.txt --output-doc-topics tutorial_composition.txt
  ```


## 07-08-18

### Más experimentación con Mallet

La exportación a Excel no funciona 100% al principio porque la nottación de los decimales en inglés se hace con puntos en lugar de comas. Hay que dar formato de texto a las celdas, pegar la info. del archivo de composición y luego cambiar el formato a número y después a porcentaje.

* El comportamiento de los tópicos por año solo puede verse si se reúnen en un solo archivo todos los materiales de un mismo año y se compara con los demás.

#### Primer ejercicio y resultados

Consolidé los datos de la carpeta "hechos" en un solo archivo por año y pedí a la aplicación que sacara un modelo de 10 tópicos. Excluí las *stopwords* según la lista empleada en el tutorial de Programming Historian. 

Modelo de tópicos:

0	0,01973	servicio acción trámite energía extracontractual contrato demanda pretensión orden demora convocada actor interpelada decisión revocarse debe daño prueba existe admitir 

1	0,02014	educación local personal alcaldesa sector colegio cuenta sed gómez les policía actividad localidad pineda manifestó año menor lugar señaló factores 

2	0,08046	cerebral efectuado vial rubio así salud magnetica electroencefalografica realizar fosyga señala paola informó impuesto haber llevó jurisdicción ley esposo finalizar 

3	0,03076	municipal camionetas sor esp codensa obras alumbrado servicio domiciliario siett pitajaya vinculación szv noviembre día domiciliarios públicos digna igualdad administración 

**4	0,37875	salud accionada entidad eps accionante acción derechos encuentra así servicios tutela médico mismo solicitó social fundamentales derecho protección antecedentes seguridad**

5	0,02002	cuenta xilena semanas general comparendos adres corte necesario recursos transporte movilidad camargo pensión cotizadas administradora dos allí ordenados traslado sistema 

6	0,03038	calidad secretaría integridad aras lacosamida lamotrigina vigente cuentas número ludivia universitario claudia riesgo constitucionales presentó cotizante procedencia dra agosto conocimiento 

7	0,08584	accidente contrato desempeñando laboral derechos marzo sumado incapacidad coordinador señor encontraba labor causa justa vital peligro habiendo circunstancias dignamente contar 

8	0,04851	hospital requeridos bolsas señaló autorización distrital tunal obstante medida humanavivir contra fondo será pos eventos cargo ips secretaría improcedencia aquella 

9	0,02091	cafesalud día oficina galindo ordenado dio relacionados física radio video legales tableta guerrero monica negativa preceptuado pasado fundación tampoco varios 

Después de pasar el archivo de composición a una hoja de cálculo, se obtuvo un gráfico de dispersión que muestra el comportamiento por año del tópico más relevante (n.° 5) durante el periodo 2009-2018. 

![_result_prueba_topico_5](https://github.com/cmvaronc/lectura-distante-tutelas/blob/master/imagen-foro-4.PNG)

|         | Tópicos |         |         |         |             |         |         |         |         |         |
| ------- | ------: | ------: | ------: | ------: | ----------: | ------: | ------: | ------: | ------: | ------: |
| **Año** |       0 |       1 |       2 |       3 |       **4** |       5 |       6 |       7 |       8 |       9 |
| 2009    | 99,473% |  0,015% |  0,059% |  0,023% |  **0,279%** |  0,015% |  0,022% |  0,063% |  0,036% |  0,015% |
| 2011    |  0,006% |  0,006% |  0,025% |  0,010% | **40,344%** |  0,006% |  0,010% |  2,244% | 57,342% |  0,007% |
| 2013    |  0,022% |  0,022% | 68,067% |  0,034% | **30,511%** |  0,022% |  0,034% |  1,210% |  0,054% |  0,023% |
| 2014    |  0,013% |  0,013% |  0,052% |  0,020% | **37,728%** |  0,013% |  0,020% | 62,097% |  0,031% |  0,014% |
| 2015    |  0,002% |  0,002% |  0,008% | 57,050% | **42,918%** |  0,002% |  0,003% |  0,008% |  0,005% |  0,002% |
| 2016    |  0,001% |  0,001% | 10,806% |  0,002% | **59,395%** |  0,001% | 12,208% |  0,069% |  0,834% | 16,681% |
| 2017    |  0,004% | 83,955% |  0,245% |  0,688% | **13,926%** |  0,005% |  1,141% |  0,019% |  0,011% |  0,005% |
| 2018    |  0,002% |  0,002% |  0,212% |  0,003% | **54,951%** | 39,298% |  0,003% |  5,520% |  0,005% |  0,002% |

Conclusiones del ejercicio:

* La muestra es muy pequeña, razón por la que la participación de los demás tópicos es muy pequeña (usualmente con valores inferiores al 1%) en comparación con el n.° 5., especialmente en los años donde hay más textos (p. ej. 2016 tiene más textos que 2009). Es imperativo agrandar el corpus para obtener valores más significativos.
* Hace falta estudiar con más detaller el algoritmo de Mallet y la manera como saca los tópicos, porque quedan preguntas sin resolver: p. ej., ¿es posible que los tópicos contengan menos *tokens*?

## 09-08-18

### Formulación de pregunta

* ¿Es factible servirse de la lingüística de corpus para hacer un diagnóstico sobre la construcción discursiva de las tutelas que ingresan al proceso de sellección de la Corte Constitucional?
* ¿Es posible mejorar el proceso de revisión de tutelas que realiza la Corte Constitucional con el apoyo de la inteligencia artificial?

Elaboramos un documento compartido en *Word Online* para consignar los apartes básicos del proyecto. 

Próxima reunión: lunes 13 de agosto, 10:00 a.m., casa de MF.

Cita con la prof. María José: 14 de agosto, 12:30 p.m.

Pendientes: continuar los análisis de prueba con las demás secciones (provisiones, consideraciones, decisiones y pretensiones).

## 11-08-18

### Clase de diseño de proyectos

Wiki del curso: hd.uniandes.edu.co/usuario/cmart/dproyecto

Repasar el documento de Drucker e inscribir el proyecto en una (o varias) de las categorías disponibles en la Wiki. 

Crear una descripción del proyecto dentro de la Wiki que debe contener lo que se encuentra en la plantilla disponible en la Wiki.

## 14-08-18

### Reunión con la profesora María José

Recolección de información: buenas prácticas de archivos no gestionados: ¿de dónde salió esto? Quizá replicar el sistema de organización que se utiliza en la corte.

Revisar el filtrado de nombres propios del catálogo de Google. Preguntar a Camilo sobre el asunto. Investigar más sobre el algoritmo.

Próxima reunión: martes 11 de septiembre, 12:00 m. Para esta, un texto que documente de forma muy breve el proceso de construcción del corpus. 2 páginas. 

## 17-08-18

### Lectura de 2 obras sobre el empleo de R como plataforma para el análisis textual

* Arnold, T. (2015). *Humanities data in R*. New York, NY: Springer Science+Business Media. 
* Desagulier, G. (2017). *Corpus Linguistics and Statistics with R*. Cham, Suiza: Springer International Publishing. [https://doi.org/10.1007/978-3-319-64572-8](https://doi.org/10.1007/978-3-319-64572-8). Revisión de los capítulos 1 y 2, que abordan temas básicos de trabajo en esta plataforma de programación. Continuar la lectura desde la página 39. Sería importante discutir con MF el tema de la representatividad de la muestra de acuerdo con los datos aportados al respecto en esta obra.

¿Cabría la posibilidad de limitar el análisis a Mallet y AntConc o definitivamente sería necesario recurrir a lenguajes más complejos, como R?

Aprendizaje básico de R: funciones básicas. Vectores, listas y matrices. La plataforma es interesante, aunque quizá pueda ser suplida por Mallet y AntConc para los propósitos introductorios del experimento. En cualquier caso, el modelado de tópicos en R también se hace con una librería de Mallet, por lo que sería redundante utilizar ambas plataformas para obtener el mismo resultado final.

## 19-08-18

### Más aprendizaje de R

* Recordar que para extraer un elemento de un dataframe se usan los corchetes cuadrados.

## 21-08-18

### Combinación de archivos .txt 

[https://www.online-tech-tips.com/free-software-downloads/combine-text-files/](https://www.online-tech-tips.com/free-software-downloads/combine-text-files/)

How to Combine or Merge Multiple Text Files

There are several occasions where you may need to merge multiple text files into single text file. For example, you may receive a CD that contains hundreds of text files, all in different directories, which you need to combine into one file for importing into Excel, etc.

It’s also useful if you have network log files, server log files, or backup logs that you want to combine for purposes of data mining or data analysis. There are a couple of different ways you can go about joining text files together and the results are slightly different depending on the method you choose.

In this article, I’ll write about several ways to combine text files so that if one method doesn’t work out too well, you can try something else.
Method 1 – Command Prompt

If you are ok using the command prompt, then there are a couple of simple commands you can use to merge a whole bunch of text files quickly. The advantage of using the command prompt is that you don’t have to install any third-party programs. If you want a little primer on using the command prompt, check out my beginner’s guide to use the command prompt.

Also, since the command line can take multiple parameters, you can really create quite a complex command to filter and sort through which files you want to include in the joining process. I’ll explain the simplest command, but will also delve into a few examples to show you how to do the more complicated stuff.

Firstly, open Windows Explorer and go to the directory where you text files are located. If the files are stored in many subfolders, navigate to the parent directory. Now press and hold CTRL + SHIFT and then right-click on any empty spot in the Explorer window.

This will open a command window that is already set to the directory  you were in. Now all we have to do is type in the command. As you can  see above, I have three text documents in the folder along with a couple  of folders. If I only want to combine the text files in this one  folder, I would issue this command:

> **for %f in (\*.txt) do type “%f” >> c:\Test\output.txt**

In coding parlance, this is a simple **FOR** loop that loops through all the files end with .TXT and outputs them to a file called **output.txt**.

As you can see above, the loop just runs a separate command for each  text file that it finds in the directory. Note that if you have a text  file, but it has a different extension like .log or .dat, etc, then you  can simply change the *.txt value in the command. It’s also worth noting  that the output should be to a different location than the current  directory, otherwise it will append the output file to itself since it  also is a text file.

Now let’s say you have text files that are located not just in one  folder, but in many subfolders. In this case, we can add a parameter to  the command, which will tell it to recursively search for text files in  any subfolders of the current directory.

> **for /R %f in (\*.txt) do type “%f” >> c:\Test\output.txt**

You’ll notice the **/R** parameter right after the for  statement. Now when I run the command, you’ll see that it finds a couple  of extra text files in the three directories that are in the same  directory.

As is usual with the command prompt, there is actually another command that allows you to do the same thing as the **FOR** statement  above. The command is actually a lot simpler and if it works fine for  you, then feel free to use it instead of the above method.

> **copy \*.txt output.txt**

This command works well, but doesn’t have as many options as the  previous command. For example, it won’t let you recursively search  through subfolders.

Method 2 – TXTCollector

**TXTCollector**  is a free text file-merging tool with a decent feature set. It’s very  easy to use and can be configured to work in a couple of different ways.

First, type or copy and paste the folder path into the **Folder** box at the top or simply click on **Browse Folders** button and select the folder with the text files. You can then choose which type of files you want to combine.

By default, TXTCollector will search for all TXT files and combine  them. However, you can pick from the list and combine or merge multiple  CSV, BAT, HTM, LOG, REG, XML, and INI files into one also!

Check the **Include subfolders** box if you want  TXTCollector to recursively look into each sub-folder of the main  folder. TXTCollector will show you exactly how many files it found in  the directory.

Next you can choose a separator that will appear between each file  that is being combined. This is a nice feature that you don’t get with  the command line method. Either you can pick from the drop down menu or  you can just type in whatever you want into the box.

By default, the program will put the directory name, file name, and  the separator between each file. If you want to combine the files  continuously without any break between each file, check off **No Separator**, **No Filename**, and **No Carriage Returns**.

You will then have the choice of adding a space character between the  files or not. The cool thing about TXTCollector is that you can really  customize it. If you click on the link at the bottom called **Extensions and Separators**, you can add your own extensions to TXTcollector.

Edit the **extensions.txt** file located in the  TXTCollector application data directory. Note that TXTcollector only  handles plain text files, no matter what extension is used.  Therefore, it cannot combine multiple XLS files, for example, unless  they are saved as plain text.

The only limitation to the program is that it can only combine 32,765  text files at once. If you have more than that, you can combine that  many into one and then combine the large one with more smaller ones, up to 32,765!

Overall, a very simple, yet powerful freeware app for combining  multiple text files. Hopefully, these two methods will work for most  people. If you have run into a situation that is more complicated, feel  free to post a comment and I’ll try to help.

## 22-08-18

### Sesión de trabajo, Diseño de proyectos

* Trabajamos en la conversión de gran volumen de archivos de texto con textutil, un script disponible de fábrica en los Mac para hacer ese trabajo. Hice posteriormente una prueba con el acervo completo de la Corte Constitucional que nos habí afacilitado Sandy y funcionó.
* La estructura de almacenamiento de la información debería modificarse: pasar de "componente-año" a "año-carpeta por tutela-archivos separados por componentes".
* El clasificador único deberá ser el número de radicación del juzgado.
* Acordamos crear el documento para entregar el 11 de septiembre, en el que se describa de qué manera se está construyendo el corpus. Este tendrá 2 apartes: de un lado, el proceso que se ha seguido para conseguir la información; y de otro, la manera como esta será almacenada y sistematizada para efectos del análisis.

## 11-09-2018

### Sesión de asesoría, María José

* Coincidimos en que no es posible trocear los archivos para hacer el modelo de tópicos por componentes.
* El trabajo abre la posibilidad de pensar en conciliar las necesidades de la Corte con la realidad de la gestión documental en los juzgados. 
* Siguiente sesión: 2 de octubre, 12:00 m.

## 15-09-2018

### Bases de datos

* Base de datos: colección de elementos organizados de forma sistemática.
* Registro: representación de un objeto real (p. ej. filas de una tabla)
* Columnas: propiedades del objeto (campos)

Tipo de dato: naturaleza de la información (numérica, lógica, de caracteres, etc.)

Una base de datos puede contener una o más tablas.

Motor de bases de datos: sistema de gestión de las bases de datos. 

* Motores de bases relacionales: vinculan una tabla con otra y hace posible hacer búsquedas que incluyan datos de 2 tablas. P. ej. MySQL, PostgSQL
* Mongo DB:  base de datos no SQL cuyos documentos no están agrupados en tablas, sino en colecciones.
* Couch DB: base de datos tipo Key Store.
* Neo 4J: base de datos tipo GraphQL. Basada en grafos.

En esta sesión, se aprendió sobre SQL y hacer peticiones a una base de datos relacional mediante una interfaz PHP My Admin

* MAMP: paquete de gestión de bases de datos. Apache (servidor Web http)
* PHP: lenguaje de programación orientado a procesar hipertexto.

## 19-09-2018

### Nomenclatura

Por facilidad, resolví usar File Renamer Basic para hacer el proceso de renombrado de todos los archivos, de acuerdo con la estructura definida en el documento de construcción del corpus. Los archivos quedaron nombrados de forma consecutiva, tomando como base la fecha de su creación. Ahora bien, es necesario entrar a definir si se quiere hacer un análisis por juzgado o solo por año. Incluso, la nomenclatura podría ampliarse para incluir no solo el nombre del juzgado sino la fecha de creación del archivo, de tal manera que sea posible analizar comportamiento mes a mes.
