# Práctica 7. Dashboard ingresos personales

## Objetivo de la práctica:
Al finalizar la práctica, serás capaz de:

- Organizar y consolidar datos de ingresos personales por categoría, periodo y producto en una estructura clara y funcional.
- Aplicar herramientas de Excel como tablas dinámicas, segmentadores y gráficos para visualizar los ingresos de forma interactiva.
- Diseñar un Dashboard visual y funcional que facilite el análisis y comparación de ingresos por año, cuatrimestre y tipo de producto.
- Interpretar los datos visualizados para identificar tendencias, patrones y apoyar la toma de decisiones financieras personales.

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

### Tarea 1. Generar tablas dinámicas con la información necesaria

Paso 1. Descargar el archivo llamado [Plantilla práctica 7](<Práctica módulo 7 dashboard.xlsx>).

Paso 2. Aparecen 3 hojas: En la hoja 1 se encuentran los datos con los que se va a trabajar; la hoja 2 llamada "PT" será el puente y la hoja 3 llamada "Dashboard_Ingreso".

Paso 3. Seleccionar los datos de la hoja "Datos Dashboard Ingresos" e inserta una tabla dinámica, llevarla a la hoja llamada "PT".

![img149](../images/img149.png)

![img150](../images/img150.png)

Paso 4. Realizar la tabla de ingresos totales.
En la sección de valores, colocar el campo "Ingresos".

![img151](../images/img151.png)

Paso 5. Cambiar el título de la tabla dinámica por "Ingresos Totales". Revisar que este en formato moneda y quitar los decimales. 

![img152](../images/img152.png)

Paso 6. Generar la tabla dinámica para poder comparar los ingresos de cada producto o fuente.
Ir a la hoja de los datos e insertar la tabla dinamica. 

![img153](../images/img153.png)

Los campos quedarán así:

- Fila --> Tipo Producto
- Valores --> Suma Ingresos

![img154](../images/img154.png)

Paso 7. Cambiar el encabezado de la columana por "Fuente de Ingresos", quitar los decimales y colocar el formato moneda.

![img155](../images/img155.png)

Paso 8. Para quitar el Total general, dirigirse a la opción de Diseño y seleccionar la opción de "Totales generales"; dar clic en la opción "Desactivado para filas y columnas".


![img156](../images/img156.png)

Paso 9. Crear una tabla que más adelante ayude a generar un gráfico de líneas para todos los años, para esto se necesita contar con los ingresos para cada año. Dirigirse a la hoja de Datos, seleccionar e insertar la tabla dinámica en la hoja "PT".
Seleccionar los campos de la siguiente manera:

- Fila --> Año
- Valores --> Suma Ingresos

![img157](../images/img157.png)

Paso 10. Cambiar el nombre de "Etiquetas de fila" por "Año", poner formato moneda, quitar los decimales y desactivar el total general.

![img158](../images/img158.png)


Paso 11. Cambiar el nombre de las tablas dinámicas para tenerlas bien identificadas.

![img159](../images/img159.png)

- Tabla 1 --> TD_Ing_Totales
- Tabla 2 --> TD_Fuentes
- Tabla 3 --> TD_Años


![img160](../images/img160.png)


### Tarea 3. Diseñar el dashboard.

Paso 1. Para pasar la tabla dinámica del total de ingresos al dashboard seleccionar la tabla y en la opción de "Analizar tabla dinámica" hacer clic en mover tabla dinámica.

![img161](../images/img161.png)

Pasar la tabla a la hoja de dashboard.

![img162](../images/img162.png)

Paso 2. Seleccionar el cuadro azul y borrarlo para poder ver la tabla. Para dar formato, subir la fuente a tamaño 20, asegurarse de que quede  en formato moneda, sin decimales y centrado. Poner letras de color blanco, centradas en negritas y un poco anchas las celdas. Usar dos tonos de azul.

![img163](../images/img163.png)

Paso 3. Crear un gráfico de la tabla Fuentes. Dirigirse a "Gráfico dinámico" y seleccionar de columnas. 

![img164](../images/img164.png)

Paso 4. Dar formato al gráfico: 
- Título: Ingreso por producto
- Eliminar el cuadro de total que aparece en el lado derecho.
- Ocultar con clic derecho el botón que aparece en la parte superior izquierda llamado "Suma de ingresos".
- Eliminar las líneas de cuadricula que aparecen de fondo.

![img165](../images/img165.png)

Paso 5. Subir el ancho de las columnas a 99% para seguir dandole formato.

![img166](../images/img166.png)


Paso 6. Agregar etiquetas en la parte superior del gráfico.
![img167](../images/img167.png)

Configurar la moneda con la clave "#,##0,"K" $".

![img168](../images/img168.png)

Subir a 10 el tamaño de las etiquetas y colocarlar en negritas. De la gráfica borrar los valores que aparecen del lado izquierdo.

![img169](../images/img169.png)


Paso 7. Mover el gráfico a la hoja donde se esta construyendo el dashboard.

![img170](../images/img170.png)

Seleccionar "Dashboard ingresos".

![img171](../images/img171.png)

Ajustar el gráfico a la parte inferior izquierda.

![img172](../images/img172.png)

Paso 8. Crear el gráfico de líneas para ver los ingresos por año.

![img173](../images/img173.png)

Dar formato al gráfico:
- Cambiar el título por: Ingresos anuales.
- Eliminar el cuadro de total que aparece en el lado derecho.
- Ocultar con clic derecho el botón que aparece en la parte superior.
- Eliminar las líneas de cuadricula que aparecen de fondo.

- Suavizar la línea de la gráfica.
![img174](../images/img174.png)

Configurar la columna donde aparecen la cifras, agregar "K" para que las cifras aparezcan así. 
![img175](../images/img175.png)

Paso 9. Mover el gráfico a la hoja de dashboard.

![img176](../images/img176.png)

Ajustar a las dimensiones que se consideraron para ese gráfico.
![img177](../images/img177.png)

### Tarea 4. Insertar segmentadores

Paso 1. Posicionarse en cualquier gráfico y seleccionar la opción de segmentadores. Marcar año, cuatrimestre y tipo de producto.

![img178](../images/img178.png)

![img179](../images/img179.png)

Paso 2. Seleccionar el segmentador de año y en la opción de columna colocar 13.

![img180](../images/img180.png)

Ajustar en el dashboard.

![img181](../images/img181.png)

Paso 3. Conectar el segmentador para que también se mueva la tabla de "Ingresos totales".

![img182](../images/img182.png)

Paso 4. Poner el gráfico estático para que no se mueva. Seleccionar el gráfico de ingreso por producto, hacer clic derecho y seleccionar "Opciones de gráfico dinámico".

![img183](../images/img183.png)

Desmarcar la opción de autoajustar para esa gráfica y para la gráfica de ingresos anuales. 

![img185](../images/img185.png)

Paso 5. Ajustar el segmentador de "Cuatrimestre" a dos columnas.

![img186](../images/img186.png)

Paso 6. Hacer lo mismo con el segmentador "Tipo Producto", colocarlo a 5 columnas y acomodarlo.

![img187](../images/img187.png)

Paso 7. Conectar el segmentador "Tipo Producto" para que la conexión quede de la siguiente manera:

![img188](../images/img188.png)

Paso 8. En cuanto a la conexión del segmentador de "Cuatrimestre" quedaría de la siguiente manera: 

![img189](../images/img189.png)


### Resultado esperado

![img190](../images/img190.png)

