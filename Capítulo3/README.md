# Modelo de datos con Power Pivot ()

## Objetivo de la práctica:
Al finalizar la práctica, serás capaz de:
- Comprender el proceso de agregar y relacionar múltiples tablas en Power Pivot para crear un modelo de datos integrado.

- Aprender a usar Power Pivot para crear una tabla dinámica basada en datos relacionados de múltiples tablas.



## Duración aproximada:
- 10 minutos.

## Escenario:
Eres un analista de datos en una empresa que maneja grandes volúmenes de información sobre ventas, productos y tiendas. Recientemente, has notado que el manejo de estos datos en hojas de Excel individuales resulta lento y complicado. Por ello, decide usar Power Pivot para integrar y relacionar estas tablas, permitiendo un análisis más fluido y eficiente.

## Instrucciones 

### Tarea 1. Agregar tablas al modelo de datos

Paso 1. Descarga y guarda el siguiente archivo llamado: [Modelos_con_Power_Pivot](Modelos_con_Power_Pivot.xlsx) 

Paso 2. Dirígete a la pestaña Ventas, posteriormente en la barra superior selecciona Power Pivot y selecciona Agregar a modelo de datos ![img46](../images/img46.png)

Verás que se despliega el editor de Power Pivot

![img47](../images/img47.png)

Paso 3. Minimizar la pantalla y hacer lo mismo con la pestaña de Tiendas y Productos
![img48](../images/img48.png)

Veras en el editor de Power Pivot las tres pestañas de cada modelo de datos agregado.

![img49](../images/img49.png)



### Tarea 2. Relacionar las tablas en Power Pivot

Paso 1. Ir a la vista de diagrama:

* En la ventana de Power Pivot, haz clic en Vista de diagrama.
* Aparecerán las tres tablas cargadas con sus encabezados visibles

![img50](../images/img50.png)

Paso 2. Relacionar la tabla de Ventas con la de Productos:
- Identifica la columna Código de Producto en ambas tablas.
- Arrastra la columna Código de Producto de la tabla de Ventas hacia la columna correspondiente en la tabla de Productos.

*Nota:* Considera que puedes arrastrar las tablas según tu preferencia.

Verifica que la relación se haya creado.

![img51](../images/img51.png)


Paso 3. Relacionar la tabla de Ventas con la de Tiendas:
- Encuentra la columna Empleado en la tabla de Ventas y la columna Empleado en la tabla de Tiendas.
- Arrastra la columna Empleado de la tabla de Ventas hacia la columna en la tabla de Tiendas.

![img52](../images/img52.png)

- Asegúrate de que la relación sea correcta.

### Tarea 3. Crear una tabla dinámica en Power Pivot

Paso 1. Insertar una tabla dinámica:
- En la ventana de Power Pivot y selecciona Tabla dinámica en la parte superior.

![img53](../images/img53.png)

- Elige Nueva hoja de cálculo para que la tabla dinámica se inserte en una hoja nueva en Excel.

Paso 2. Agregar campos a la tabla dinámica:
- En la lista de campos de la tabla dinámica, selecciona Tienda de la tabla de Tiendas y colócala en el área de Filas.
- Agrega Descripción del Producto de la tabla de Productos al área de Filas debajo de Tienda.
Añade Unidades de la tabla de Ventas al área de Valores. 
![img54](../images/img54.png)

Paso 3. Guarda los cambios realizados y cierra el archivo.

### Resultado esperado

![img55](../images/img55.png)


# Filtrado Interactivo de Ventas con Segmentación en Power Pivot 

## Objetivo de la práctica:
Al finalizar la práctica, serás capaz de:

- Crear una tabla dinámica basada en el modelo de datos para analizar ventas de forma detallada por empleado y categoría de producto.

- Aplicar segmentaciones de datos para filtrar dinámicamente los resultados en la tabla dinámica, mejorando la interacción y el análisis visual.

## Duración aproximada:
- 15 minutos.

## Instrucciones 

### Tarea 1. Generar modelo de datos

Paso 1: Descarga el archivo llamado [Práctica_2_módulo_3](práctica_módulo_3_parte_2.xlsx)

Paso 2: En la pestaña "empleados" seleccionar la tabla , en la parte superior ir a power pivot y dar clic en agregar a modelo de datos.

![img56](../images/img56.png)

Confirmamos 

![img57](../images/img57.png)

Paso 3. Cerrramos la hoja y repetimos lo mismo con cada una de las tablas de la pestaña "Ventas" y "Categoría"


![img58](../images/img58.png)

Paso 4. Una vez que ya está todas las tablas en power pivot, cambiamos los nombres de las tablas, dando clic derecho en la opción cambiar nombre.


![img59](../images/img59.png)

Los nombre deben quedar de la siguiente manera: 

![img60](../images/img60.png)

Paso 5. Vamos a la opción de vista de diagrama en Power Pivot.

![img61](../images/img61.png)

Paso 6. Creamos las relaciones de la siguiente manera: 
- Tabla empleados (código) va a unirse a tabla ventas (código)
- Tabla Ventas (categoría) va a unirse a tabla categoría (categoría)

![img62](../images/img62.png)


### Tarea 2. Crear tabla dinánmica

Paso 1. En la barra superior seleccionamos tabla dinámica

![img63](../images/img63.png)

Paso 2. Selecciona una nuneva hoja de calculo.
![img64](../images/img64.png)

Paso 3. La tabla dinámica quedará en la columnas el campo de "Nombre" que está en la tabla empleados.
Las filas quedarán con el campo Fecha (de la tabla ventas), categoría( de la tabla categoría) y productos (de la tabla Ventas)

En valores quedará la suma del campo total que está en la tabla "Ventas"

![img65](../images/img65.png)

Paso 4. Vamos a la celda donde aparece la primera fecha que es 04/05/2020
damos clic derecho y seleccionamos agrupar.

![img66](../images/img66.png)

Seleccionamos la opción de meses y aceptar.

![img67](../images/img67.png)

Paso 5. seleccionamos una celda de la columna del total general, clic derecho y vamos a formato número

![img68](../images/img68.png)

Pao 6. Seleccionamos el formato moneda y las posiciones decimales 0.
![img69](../images/img69.png)


### Tarea 3. Insertar segmentadores

Paso 1. Nos posicionamos en la tabla dinámica y vamos a en la barra superiro a la opción de "Analizar tabla dinámica" y seleccionamos "Insertar segmentación de datos"
![img70](../images/img70.png)

Paso 2. Vamos a seleccionar en la tabla categoría la opción categoría. Y en la tabla ventas seleccionamos productos.


![img71](../images/img71.png)

![img72](../images/img72.png)

Paso 3. En los segmentadores insertados, seleccionamos "consumo básico" y "azúcar" y "café"

Paso 4: Guarda los cambios realizados y cierra el archivo.

*Nota:* Si deseas puedes cambiar el color de los segmentadores o de la tabla dinámica. Para esto hay que ir a la opción Diseño.
![img74](../images/img74.png)
![img75](../images/img75.png)

### Resultado esperado
![img73](../images/img73.png)


# Evaluación de Ventas con KPIs en Power Pivot

## Objetivo de la práctica:
Al finalizar la práctica, serás capaz de:

- Integrar datos comerciales al modelo de Power Pivot.

-Crear una medida DAX que calcule el promedio de ventas por operación.

-Construir un KPI visual para evaluar el cumplimiento de metas de venta por producto.

-Analizar gráficamente los resultados mediante una tabla dinámica.

## Duración aproximada:
- 15 minutos.

## Escenario:
Trabajas en el área de inteligencia comercial de una empresa dedicada a la distribución de tecnología, mobiliario y telecomunicaciones a nivel nacional. Cada venta tiene un valor considerable, ya que se trata de productos empresariales.

La gerencia solicita un informe visual que indique qué productos están cumpliendo con el objetivo de ventas promedio por operación, fijado en $6,000 MXN.

Para ello, vas a construir un KPI con Power Pivot, el cual te permitirá visualizar este rendimiento con indicadores de color.

## Instrucciones 

### Tarea 1.Cargar los datos al modelo de Power Pivot

Paso 1. Descargar y abrir el archivo [Práctica_módulo_3_ parte_3](práctica_módulo3_parte_3.xlsx)

Paso 2. Convierte los datos en una tabla (Crtl + T) y nombrala VentasKPI

![img76](../images/img76.png)
![img77](../images/img77.png)

Paso 3. Ve a la pestaña Power Pivot > Agregar al modelo de datos.

![img78](../images/img78.png)

### Tarea 2.Crear una medida de Promedio de Venta

Paso 1. Da formato de moneda a la columna Precio y columna Total

![img79](../images/img79.png)

Paso 2. En el área de cálculo, crea una medida con la siguiente formula :

![img80](../images/img80.png)

*PromedioVenta := AVERAGE(VentasKPI[Total])*

![img81](../images/img81.png)

Paso 3. Dale formato al promedio de venta, dar clic derecho, opción formato. Seleccionar Moneda, simbolo $ y posiciones decimales 1.

![img82](../images/img82.png)


### Tarea 3.Crear el KPI

Paso 1. Selecciona la medida de PromedioVenta
Paso 2. Haz clic en "Crear KPI" en la pestaña de Inicio de Power Pivot
![img83](../images/img83.png)

Paso 3. Configura el KPI así:

Valor objetivo absoluto: 6000

Indicadores de estado:

🔴 Rojo si < 4000

🟡 Amarillo si entre 4000 y 6000

🟢 Verde si > 6000

Paso 4. Confirma con Aceptar

![img84](../images/img84.png)

### Tarea 34.  Crear una tabla dinámica para visualizar

Paso 1. Regresa a tu hoja de excel donde esta la tabla  y selecciona la opción de insertar tabla dinámica, selecciona la opción de "Desde modelo de datos" y en una nueva hoja 

![img85](../images/img85.png)

Paso 2. En la tabla dinámica:

- Agrega Producto a Filas.

- Agrega a Valores:

    - Promedio de venta

    - Estado del KPI (el icono visual)

![img86](../images/img86.png)

Paso 3. Guardamos los cambios y cerramos el libro.

### Resultado esperado
![img87](../images/img87.png)
