# Dashboard Ingresos Personales

## Objetivo de la práctica:
Al finalizar la práctica, serás capaz de:

-Organizar y consolidar datos de ingresos personales por categoría, periodo y producto en una estructura clara y funcional.

-Aplicar herramientas de Excel como tablas dinámicas, segmentadores y gráficos para visualizar los ingresos de forma interactiva.

-Diseñar un Dashboard visual y funcional que facilite el análisis y comparación de ingresos por año, cuatrimestre y tipo de producto.

-Interpretar los datos visualizados para identificar tendencias, patrones y apoyar la toma de decisiones financieras personales.



## Escenario:
Ana es una profesional independiente que desde 2010 ha generado ingresos por diferentes medios: Alquiler, Cursos, Eventos, Libros y Trabajos. Ha llevado un registro trimestral de cada ingreso en euros, y ahora desea tener una visión clara y visual de su evolución financiera.

Situación:
Ana quiere consolidar toda su información en un Dashboard interactivo que le permita:

- Ver sus ingresos anuales totales.

- Comparar ingresos por tipo de producto.

- Detectar qué trimestre del año le genera mayores ingresos.

- Identificar tendencias a lo largo del tiempo.

## Duración aproximada:
- 25 minutos.


## Instrucciones 

### Tarea 1. Generar tablas dinámicas con la información necesaria.

Paso 1. Descarga el archivo llamado [Plantilla práctica 7](<Práctica módulo 7 dashboard.xlsx>)

Paso 2. Verás 3 hojas, en la hoja 1 aparecen los datos con los que vamos a trabajar, la hoja 2 llamada "PT" que será el puente y la hoja llamada "Dashboard_Ingreso"

Paso 3. Seleccionamos los datos de la hoja "Datos Dashboard Ingresos" e inserta una tabla dinámica, llevala a la hoja llamada "PT"

![img149](../images/img149.png)

![img150](../images/img150.png)

Paso 4. Vamos a realizar la tabla de ingresos totales
En la sección de valores, colocamos el campo "Ingresos"


![img151](../images/img151.png)

Paso 5. Cambiamos el título de la tabla dinámica. por "Ingresos Totales". Revisar que este en formato moneda y quitamos los decimales. 

![img152](../images/img152.png)

Paso 6. Vamos a generar la tabla dinámica para comparar los ingresos para cada producto o fuente.
Vamos a la hoja de los datos, insertar tabla dinamica 

![img153](../images/img153.png)

Los campos quedarán así:
Fila --> Tipo Producto
Valores --> Suma Ingresos

![img154](../images/img154.png)

Paso 7. Cambiamos el encabezado de la columana por "Fuente de Ingresos", quitamos los decimales y colocamos el formato moneda.

![img155](../images/img155.png)

Paso 8. Vamos a quitar el total general.Vamos a la opción de Diseño. Seleccionamos la opción de "Totales generales" y damos clic en la opción "Desactivado para filas y columnas"


![img156](../images/img156.png)

Paso 9. Vamos a crear una tabla que nos ayude más adelante a generar un gráfico de líneas para todos los años, así que necesitamos los ingresos para cada año. Vamos a la hoja de Datos, seleccionamos e insertamos la tabla dinámica en la hoja "PT".
Seleccionamos los campos de la siguiente manera

Fila --> Año
Valores --> Suma Ingresos

![img157](../images/img157.png)

Paso 10. Cambiamos el nombre de "Etiquetas de fila" por "Año", ponemos formato moneda, quitamos los decimales y desactivamos el total general.

![img158](../images/img158.png)


Paso 11. Vamos a cambiar el nombre de las tablas dinámicas para tenerlas bien identificadas.
Vamos a la primera 
![img159](../images/img159.png)

- Tabla 1 --> TD_Ing_Totales
- Tabla 2 --> TD_Fuentes
- Tabla 3 --> TD_Años


![img160](../images/img160.png)


### Tarea 3. Diseñar el dashboard.

Paso 1. Vamos a pasar la tabla dinámica del total de ingresos al dashboard. Seleccionamos la tabla y en la opción de Analizar tabla dinámica y escogemos mover tabla dinámica.

![img161](../images/img161.png)

Pasamos la tabla a la hoja de dashboard

![img162](../images/img162.png)

Paso 2. Seleccionamos el cuadro azul y lo borramos para poder ver la tabla. Damos formato, le subimos la fuente a tamaño 20, nos aseguramos que quede  en formato moneda, sin decimales y centrado. Ponemos letras de color blanco, centrada en negritas y un poco ancho las celda. Usar dos tonos de azul.

![img163](../images/img163.png)

Paso 3. Vamos a crear un gráfico de la tabla Fuentes. Vamos a gráfico dinámico y seleccionamos de columnas. 

![img164](../images/img164.png)

Paso 4. Dar formato al gráfico: 
- Título: Ingreso por producto
- Eliminar el cuadro de total que aparece en el lado derecho.
- Ocultamos con clic derecho el botón que aparece en la parte superior izquierda llamado "Suma de ingresos"
- Eliminamos las líneas de cuadricula que aparecen de fondo

![img165](../images/img165.png)

Paso 5. Seguimos dando formato, subimos el ancho de las columnas a 99%

![img166](../images/img166.png)


Paso 6. Agregamos etiquetas en la parte superior del gráfico.
![img167](../images/img167.png)

Configuramos la moneda con la clave "#,##0,"K" $"

![img168](../images/img168.png)

Las etiquetas les subimos el tamaño a un 10, en negritas. De la grafica borramos los valore que aparecen del lado izquierdo.

![img169](../images/img169.png)


Paso 7. Movemos el gráfico a la hoja donde estamos construyendo el dashboard.

![img170](../images/img170.png)

Seleccionamos dashboard ingresos

![img171](../images/img171.png)

Ajustamos el gráfico a la parte inferior izquierda

![img172](../images/img172.png)

Paso 8. Ahora vamos a crear el gráfico de líneas para ver los ingresos por año.

![img173](../images/img173.png)

Dar formato al gráfico:
- El titulo lo cambiamos por: Ingresos anuales.
- Eliminar el cuadro de total que aparece en el lado derecho.
- Ocultamos con clic derecho el botón que aparece en la parte superior.
- Eliminamos las líneas de cuadricula que aparecen de fondo

- Suavisamos la línea de la gráfica.
![img174](../images/img174.png)

Configuramos la columna donde aparecen la cifras, agregamos "K" para que las cifras aparezcan así. 
![img175](../images/img175.png)

Paso 9. Movemos el gráfico a la hoja de dashboard.

![img176](../images/img176.png)

Ajustamos a las dimensiones que se consideraron para ese gráfico.
![img177](../images/img177.png)

### Tarea 4. Insertar segmentadores

Paso 1. Nos posicionamos en cualquier gráfico y seleccionamos la opción de segmentadores. Marcamos año, cuatrimestre, tipo de producto

![img178](../images/img178.png)

![img179](../images/img179.png)

Paso 2. Seleccionamos el segmentador de año y en la opción de columna colocamos 13.

![img180](../images/img180.png)

Ajustamos en el dashboard.

![img181](../images/img181.png)

Paso 3. Vamos a conectar ese segmentador para que también se mueva la tabla de "Ingresos totales"

![img182](../images/img182.png)

Paso 4. Vamos a poner el gráfico estático para que no se muevan. Seleccionamos el gráfico de ingreso por producto, clic derecho y seleccionamos "Opciones de gráfico dinámico"

![img183](../images/img183.png)

Desmarcamos la opción de autajustar para esa gráfica y para la gráfica de ingresos anuales. 

![img185](../images/img185.png)

Paso 5. Agustamos el segmentador de Cuatrimestre a dos columnas.

![img186](../images/img186.png)

Paso 6. Hacemos lo mismo con el segmentador tipo de producto, lo colocamos a 5 columnas y acomodamos.

![img187](../images/img187.png)

Paso 7. Vamos a conectar el segmentador tipo de producto que quede de la siguiente manera la conexión.

![img188](../images/img188.png)

Paso 8. Vamos con la conexión del segmentador de cuatrimestre que quedaría de la siguiente manera: 

![img189](../images/img189.png)


### Resultado esperado

![img190](../images/img190.png)

