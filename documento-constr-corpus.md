# Construcción de corpus para el análisis

## 1. Consecución de la información

## 2. Composición del corpus

### 2.1. Diseño de la muestra

Vista la envergadura del universo de información que se enfrenta en un ejercicio de investigación – creación como el propuesto, ha sido claro desde el inicio que el volumen de documentos que compondrían la muestra sería arbitrario. Así entonces, la representatividad de la muestra no estará dada por el valor numérico absoluto frente a la totalidad del universo de información, sino por la capacidad que esta tenga para reflejar las tendencias de uso de la lengua (de acuerdo con la conceptualización de Biber [1991]) que, a posterioridad, se evidenciarán mediante el modelado de tópicos.

Nótese en este punto que la jurisprudencia emitida por la Corte Constitucional desde su creación (en 1991) asciende a 25.000 documentos, aproximadamente. Con esto, y para atender lo expresado en el párrafo anterior, se tomó la decisión de componer una muestra aleatorizada de 15 fallos de tutela por cada año de existencia de la Corte, obtenidos a partir de los archivos recabados en las visitas a las sedes judiciales. La muestra, entonces, ostentará una envergadura equivalente al 1,56 % del total de documentos que componen la jurisprudencia de la Corte.

El hecho de que los fallos de tutela ostenten secciones cuya construcción obedece a tipologías textuales disímiles (narrativa, descriptiva y argumentativa) podría sesgar los resultados del modelado de tópicos. Por tal motivo, se había tomado en principio la decisión de separarlos por componentes (i. e. consideraciones, hechos, pretensiones, decisiones), de tal manera que se produjera un modelo de tópicos para cada uno. Ahora bien, dado que la acción de dividir estos documentos no puede automatizarse y, por lo tanto, excede la capacidad humana de la cual se dispone para realizar el experimento, se tomó la decisión de descartar esta acción y limitarse a tomar para el análisis los archivos de los fallos sin dividirlos.

### 2.2. Sistematización de la muestra

Tras haber establecido las características generales de la muestra, corresponde tomar decisiones respecto de la manera como se organizará el acervo de información para el análisis; a continuación, se describen con más detalle estos asuntos.

#### 2.2.1. Formato

El algoritmo que se empleará para construir el modelo de tópicos (Mallet) exige trabajar con archivos de texto plano y codificación Unicode (UTF-8). Ahora bien, dado el carácter desestructurado de la información de la muestra (archivos en formatos de texto enriquecido, en incluso de imagen), se ha hecho necesario buscar herramientas digitales que permitan convertirla de forma eficiente y confiable al formato requerido. En consecuencia, se decidió emplear para este menester la aplicación Textutil: se trata de un paquete de servicios para la conversión de archivos de texto que se ejecuta en la terminal del sistema operativo Mac OS X. Aparte de haber mostrado resultados satisfactorios en ejercicios preliminares (realizados con el corpus de prueba), se destaca de otras aplicaciones de su tipo en tanto permite convertir directorios completos.  

#### 2.2.2. Gestión de archivos

Encontrar un elemento que sirviese como clasificador único para nombrar los archivos ha resultado ser una tarea más complicada de lo que se pensó en principio. En este sentido, se creyó prudente recurrir a la clasificación dada desde los juzgados a los expedientes, con lo cual se tomarán los siguientes elementos para nombrar los archivos:

![nomenclatura-archivos](https://github.com/cmvaronc/lectura-distante-tutelas/blob/master/nomenclatura-archivos.png)
 
La configuración de una estructura de carpetas para el almacenamiento de los archivos, por su parte, tampoco ha estado exenta de discusiones. Se resolvió disponer carpetas para almacenenar los fallos a analizarse por año:

![estructura-archivos](https://github.com/cmvaronc/lectura-distante-tutelas/blob/master/estructura-archivos.png)
 
## Referencias
Biber, D. (1993). Representativeness in Corpus Design. *Literary and Linguistic Computing, 8*(4), 243–257. https://doi.org/10.1093/llc/8.4.243

