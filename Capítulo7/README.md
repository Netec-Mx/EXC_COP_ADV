# Práctica 7. Dashboard ingresos personales

## Objetivo de la práctica:
Al finalizar la práctica, serás capaz de:

- Organizar y consolidar datos de ingresos personales por categoría, periodo y producto en una estructura clara y funcional.
- Aplicar herramientas de Excel como tablas dinámicas, segmentadores y gráficos para visualizar los ingresos de forma interactiva.
- Diseñar un Dashboard visual y funcional que facilite el análisis y comparación de ingresos por año, cuatrimestre y tipo de producto.
- Interpretar los datos visualizados para identificar tendencias, patrones y apoyar la toma de decisiones financieras personales.

## Duración aproximada:
- 25 minutos.

---

**[⬅️ Atrás](https://netec-mx.github.io/EXC_COP_ADV/Cap%C3%ADtulo6/)** | **[Lista General](https://netec-mx.github.io/EXC_COP_ADV/)** | **[Siguiente ➡️](https://netec-mx.github.io/EXC_COP_ADV/Cap%C3%ADtulo8/)**

---

## Escenario:
Ana es una profesional independiente que desde 2010 ha generado ingresos por diferentes medios: Alquiler, Cursos, Eventos, Libros y Trabajos. Ha llevado un registro trimestral de cada ingreso en euros, y ahora desea tener una visión clara y visual de su evolución financiera.

**Situación:**

Ana quiere consolidar toda su información en un Dashboard interactivo que le permita:

- Ver sus ingresos anuales totales.
- Comparar ingresos por tipo de producto.
- Detectar qué trimestre del año le genera mayores ingresos.
- Identificar tendencias a lo largo del tiempo.

## Instrucciones:

### Tarea 1. Generar tablas dinámicas con la información necesaria.

Paso 1. Descarga el archivo llamado [Plantilla práctica 7](<Práctica módulo 7 dashboard.xlsx>).

Paso 2. Aparecen 3 hojas: En la hoja 1 se encuentran los datos con los que vas a trabajar. La hoja 2, llamada "PT", será el puente; y la hoja 3, llamada "Dashboard_Ingreso".

Paso 3. Selecciona los datos de la hoja "Datos Dashboard Ingresos" e inserta una tabla dinámica. Posteriormente, llévala a la hoja llamada **PT**.

![img149](../images/img149.png)

![img150](../images/img150.png)

Paso 4. Realiza la tabla de **ingresos totales**.

En la sección de valores, coloca el campo "Ingresos".

![img151](../images/img151.png)

Paso 5. Modifica el título de la tabla dinámica por "Ingresos Totales". Revisa que se encuentre en formato **moneda** y quita los decimales. 

![img152](../images/img152.png)

Paso 6. Genera la tabla dinámica para comparar los ingresos de cada producto o fuente.

Dirígete a la hoja de los datos e inserta la tabla dinámica. 

![img153](../images/img153.png)

Por lo tanto, los campos quedarán de la siguiente forma:

- Fila ➡️ Tipo Producto
- Valores ➡️ Suma Ingresos

![img154](../images/img154.png)

Paso 7. Cambia el encabezado de la columana por "Fuente de Ingresos", quita los decimales y coloca el formato moneda.

![img155](../images/img155.png)

Paso 8. Para quitar el total general, dirígete a la opción de "Diseño" y selecciona la opción de "Totales generales"; da clic en la opción "Desactivado para filas y columnas".

![img156](../images/img156.png)

Paso 9. Crea una tabla, la cual más adelante ayude a generar un gráfico de líneas para todos los años; para esto se necesita contar con los ingresos para cada año. 

Dirígete a la hoja de "Datos", selecciona e inserta la tabla dinámica en la hoja PT.

Selecciona los campos de la siguiente manera:

- Fila ➡️ Año
- Valores ➡️ Suma Ingresos

![img157](../images/img157.png)

Paso 10. Sustituye el nombre de "Etiquetas de fila" por "Año", asigna el formato moneda, quita los decimales y desactiva el total general.

![img158](../images/img158.png)

Paso 11. Cambia el nombre de las tablas dinámicas para que puedan ser identificadas más facilmente.

![img159](../images/img159.png)

- Tabla 1 ➡️ TD_Ing_Totales
- Tabla 2 ➡️ TD_Fuentes
- Tabla 3 ➡️ TD_Años

![img160](../images/img160.png)

### Tarea 2. Diseñar el dashboard.

Paso 1. Para pasar la tabla dinámica del total de ingresos al dashboard, selecciona la tabla y, en la opción de "Analizar tabla dinámica", haz clic en mover tabla dinámica.

![img161](../images/img161.png)

Pasa la tabla a la hoja de dashboard.

![img162](../images/img162.png)

Paso 2. Selecciona el cuadro azul y elimínalo para poder ver la tabla. Para dar formato, aumenta la fuente a tamaño 20. También, asegúrate de que quede en formato moneda, sin decimales y centrado. Pon letras de color blanco, centradas y en negritas, y un poco anchas las celdas. Asimismo, utiliza dos tonos de azul.

![img163](../images/img163.png)

Paso 3. Crea un gráfico de la tabla "Fuentes". Dirígete a "Gráfico dinámico" y selecciona la opción de "Columnas". 

![img164](../images/img164.png)

Paso 4. Da formato al gráfico: 
- Título: Ingreso por producto.
- Elimina el cuadro de total que aparece en el lado derecho.
- Oculta con clic derecho el botón que aparece en la parte superior izquierda llamado "Suma de ingresos".
- Elimina las líneas de cuadricula que aparecen de fondo.

![img165](../images/img165.png)

Paso 5. Aumenta el ancho de las columnas a 99% para continuar dándole formato.

![img166](../images/img166.png)

Paso 6. Agrega etiquetas en la parte superior del gráfico.

![img167](../images/img167.png)

Configura la moneda con la clave `"#,##0,"K" $"`.

![img168](../images/img168.png)

Aumenta a 10 el tamaño de las etiquetas y colócalas en negritas. De la gráfica, borra los valores que aparecen del lado izquierdo.

![img169](../images/img169.png)

Paso 7. Desplaza el gráfico a la hoja donde se está construyendo el dashboard.

![img170](../images/img170.png)

Selecciona "Dashboard ingresos".

![img171](../images/img171.png)

Ajusta el gráfico a la parte inferior izquierda.

![img172](../images/img172.png)

Paso 8. Crea el gráfico de líneas para observar los ingresos por año.

![img173](../images/img173.png)

Proporciona formato al gráfico:
- Cambia el título por: Ingresos anuales.
- Eliminr el cuadro de total que aparece en el lado derecho.
- Oculta con clic derecho el botón que aparece en la parte superior.
- Elimina las líneas de cuadricula que aparecen de fondo.
- Suaviza la línea de la gráfica.

![img174](../images/img174.png)

Configura la columna donde aparecen la cifras, agrega "K" para que las cifras aparezcan así. 

![img175](../images/img175.png)

Paso 9. Mueve el gráfico a la hoja de dashboard.

![img176](../images/img176.png)

Ajusta a las dimensiones que se consideraron para ese gráfico.

![img177](../images/img177.png)

### Tarea 3. Insertar segmentadores.

Paso 1. Posiciónate en cualquier gráfico y selecciona la opción de "Segmentadores"; marca: Año, Cuatrimestre y Tipo de producto.

![img178](../images/img178.png)

![img179](../images/img179.png)

Paso 2. Selecciona el segmentador de año y, en la opción de "Columna", coloca 13.

![img180](../images/img180.png)

Ajusta en el dashboard.

![img181](../images/img181.png)

Paso 3. Conecta el segmentador para que también se mueva la tabla de "Ingresos totales".

![img182](../images/img182.png)

Paso 4. Coloca el gráfico estático para que éste no se mueva. 

Selecciona el gráfico de ingreso por producto, haz clic derecho y selecciona "Opciones de gráfico dinámico".

![img183](../images/img183.png)

Desmarca la opción de autoajustar para esa gráfica y para la de "Ingresos anuales". 

![img185](../images/img185.png)

Paso 5. Ajusta el segmentador de "Cuatrimestre" a dos columnas.

![img186](../images/img186.png)

Paso 6. Realiza lo mismo con el segmentador "Tipo Producto", colócalo a 5 columnas y acomódalo.

![img187](../images/img187.png)

Paso 7. Conecta el segmentador **Tipo Producto** para que la conexión quede de la siguiente manera:

![img188](../images/img188.png)

Paso 8. En cuanto a la conexión del segmentador de **Cuatrimestre**, quedaría de la siguiente manera: 

![img189](../images/img189.png)

## Resultado esperado:

![img190](../images/img190.png)
