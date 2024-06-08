Defunciones por cáncer en México
================
Estudiante
2024-02-06

# Instrucciones

Este reporte trata sobre las defunciones por cáncer en México, y se está
enfocando en defunciones para un estado en particular. La idea es que
las estudiantes realicen su propio análisis de los datos disponibles,
pero se pueden ofrecer las siguientes pautas para dar una orientación al
trabajo:

## Introducción

- Presentar una introducción haciendo referencia al cáncer, tipos del
  mismo y prevalencia en México según cifras oficiales. Informar que
  estos datos corresponden a base de datos abiertos en [Mortalidad de
  INEGI](https://www.inegi.org.mx/programas/mortalidad/#datos_abiertos)
  para el año 2021.

## Resultados

- Presentar un comparativo a nivel nacional (gráfico de barras) para ver
  el número de defunciones de cáncer para hombres y mujeres. Interpretar
  resultados.

  - Considerar la clave para identificar sexo es 1 para Hombre, 2 para
    Mujer y 9 para No especificado.

- Presentar gráfico de calor para comparar el número de defunciones de
  cáncer en los diferentes estados del país y por sexo. Interpretar
  resultados.

- Presentar un gráfico de barras para comparar el número de defunciones
  de cada tipo de cáncer en el estado seleccionado por el usuario. Se
  usará la columna *“causa_def”* como base para este resumen de
  información. La interpretación se hace junto con la siguiente tabla.

- Presentar una tabla que indique el número de defunciones para cada
  tipo de cáncer en la entidad seleccionada por el usuario. Se usará la
  columna *“causa_def”* como base para este resumen de información.
  Interpretar resultados.

- Calcular una columna de edad (*“anio_ocur”* - *“anio_nacim”*) y una
  gráfica de grupo etario (e.g. cada 20 años). Presentar una gráfica de
  calor en donde se compare el número de defunciones por grupo etario y
  sexo en el estado seleccionado por el usuario. Interpretar resultados.

- Es importante resaltar que el reporte se hace de manera automática,
  entonces la interpretación **(sobre todo en los datos por estado)**
  debe utilizar secciones de código que extraigan valores de los juegos
  de datos e incluso sentencias `ifelse`, para mantenerse apegada a las
  cifras.

## Conclusión

- Dictar alguna sugerencia general sobre el estado de salud de la gente
  en el país, o bien hacer alguna última comparación entre los números
  de defunciones a nivel estado y a nivel nacional.

# Códigos de ejemplo

- Comparativa nacional por sexo

![](Sesion3_Proyecto_files/figure-gfm/defun_nacional_sexo-1.png)<!-- -->

- Comparativa nacional por estados y por sexo
  - Se puede filtrar Sexo No especificado, para que la gráfica tenga
    mejor presentación.

![](Sesion3_Proyecto_files/figure-gfm/defun_nacional_estados_sexo-1.png)<!-- -->

- Gráfico de barras para el estado seleccionado.
  - Debido a la cantidad de categorías de tipos de cáncer disponibles,
    se recomienda hacer esta gráfica interactiva con plotly, para poder
    obtener algo de información de su visualización.

![](Sesion3_Proyecto_files/figure-gfm/defun_estado_%20tipocancer_grafica-1.png)<!-- -->

- Tabla de defunciones por cada tipo de cáncer

![](Sesion3_Proyecto_files/figure-gfm/defun_estado_tipocancer_tabla-1.png)<!-- -->

- **Ejemplo de interpretación:** El tipo de cáncer que más muertes causa
  en el estado de Tabasco es C61X con un total de 143 defunciones. Le
  siguen C229, C509, C169 y C189, con 135, 128, 124 y 101 defunciones,
  respectivamente.

- Defunciones por edad y sexo

![](Sesion3_Proyecto_files/figure-gfm/defun_estado_edadsexo-1.png)<!-- -->

- **Ejemplo de interpretación:** El grupo poblacional que registra mayor
  número de defunciones por cáncer son hombres viviendo hasta pasados
  los 70s. Le siguen hombres en sus 60s y por último mujeres en sus 70s.
  Entre estos tres grupos suman 525 decesos, que equivalen al
  34.0687865% del total de defunciones por cáncer en Tabasco.
