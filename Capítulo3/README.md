# Nombre del laboratorio 

## Objetivo de la práctica:
Al finalizar la práctica, serás capaz de:
- Objetivo1
- Objetivo2
- Objetivo3



## Duración aproximada:
- xx minutos.

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


### Resultado esperado

![img55](../images/img55.png)
