# Práctica 3.1. Modelo de datos con Power Pivot

## Objetivo de la práctica:
Al finalizar la práctica, serás capaz de:
- Comprender el proceso de agregar y relacionar múltiples tablas en Power Pivot para crear un modelo de datos integrado.
- Aprender a usar Power Pivot para crear una tabla dinámica basada en datos relacionados de múltiples tablas.

## Duración aproximada:
- 10 minutos.

---

**[⬅️ Atrás](https://netec-mx.github.io/EXC_COP_ADV/Cap%C3%ADtulo2/)** | **[Lista General](https://netec-mx.github.io/EXC_COP_ADV/)** | **[Siguiente ➡️](https://netec-mx.github.io/EXC_COP_ADV/Cap%C3%ADtulo4/)**

---

## Escenario:
Eres un analista de datos en una empresa que maneja grandes volúmenes de información sobre ventas, productos y tiendas. Recientemente, has notado que el manejo de estos datos en hojas de Excel individuales resulta lento y complicado. Por ello, decides usar Power Pivot para integrar y relacionar estas tablas, permitiendo un análisis más fluido y eficiente.

## Instrucciones:

### Tarea 1. Agregar tablas al modelo de datos.

Paso 1. Descarga y guarda el siguiente archivo: [Modelos_con_Power_Pivot](Modelos_con_Power_Pivot.xlsx). 

Paso 2. En la pestaña "Ventas", selecciona Power Pivot en la barra superior y haz clic en "Agregar a modelo de datos" 

![img46](../images/img46.png).

De esta forma, puedes observar el despliegue del editor de Power Pivot.

![img47](../images/img47.png)

Paso 3. Minimiza la pantalla y realiza lo mismo con la pestaña de "Tiendas" y "Productos".

![img48](../images/img48.png)

En el editor de Power Pivot se observan las tres pestañas de cada modelo de datos agregado.

![img49](../images/img49.png)


### Tarea 2. Relacionar las tablas en Power Pivot.

Paso 1. Ve a la vista de diagrama:

- En la ventana de Power Pivot, haz clic en "Vista de diagrama".
- Aparecerán las tres tablas cargadas con sus encabezados visibles.

![img50](../images/img50.png)

Paso 2. Relaciona la tabla de **Ventas** con la de **Productos**:
- Identifica la columna "Código de Producto" en ambas tablas.
- Arrastra la columna "Código de Producto" de la tabla de **Ventas** hacia la columna correspondiente en la tabla de **Productos**.

> Nota: Considera que puedes arrastrar las tablas según tu preferencia.

Verifica que la relación se haya creado.

![img51](../images/img51.png)

Paso 3. Relaciona la tabla de **Ventas** con la de **Tiendas**:
- Encuentra la columna "Empleado" en la tabla de Ventas y la columna "Empleado" en la tabla de Tiendas.
- Arrastra la columna "Empleado" de la tabla de Ventas hacia la columna en la tabla de Tiendas.

![img52](../images/img52.png)

- Asegúrate de que la relación sea correcta.

### Tarea 3. Crear una tabla dinámica en Power Pivot.

Paso 1. Inserta una tabla dinámica:
- En la ventana de Power Pivot, selecciona "Tabla dinámica" en la parte superior.

![img53](../images/img53.png)

- Elige "Nueva hoja de cálculo" para que la tabla dinámica se inserte en una hoja nueva en Excel.

Paso 2. Agrega campos a la tabla dinámica:
- En la lista de campos de la tabla dinámica, selecciona "Tienda" de la tabla de "Tiendas" y colócala en el área de "Filas".
- Agrega "Descripción del Producto" de la tabla de Productos al área de Filas debajo de Tienda.
- Añade "Unidades" de la tabla de Ventas al área de "Valores". 

![img54](../images/img54.png)

Paso 3. Guarda los cambios realizados y cierra el archivo.

## Resultado esperado:

![img55](../images/img55.png)

---

# Práctica 3.2. Filtrado interactivo de ventas con segmentación en Power Pivot 

## Objetivo de la práctica:
Al finalizar la práctica, serás capaz de:

- Crear una tabla dinámica basada en el modelo de datos para analizar ventas de forma detallada por empleado y categoría de producto.
- Aplicar segmentaciones de datos para filtrar dinámicamente los resultados en la tabla dinámica, mejorando la interacción y el análisis visual.

## Duración aproximada:
- 15 minutos.

## Instrucciones:

### Tarea 1. Generar modelo de datos.

Paso 1. Descarga el archivo [Práctica_2_módulo_3](práctica_módulo_3_parte_2.xlsx).

Paso 2. En la pestaña "Empleados", selecciona la tabla y, en la parte superior, ve a Power Pivot. Da clic en "Agregar a modelo de datos".

![img56](../images/img56.png)

Confirma.

![img57](../images/img57.png)

Paso 3. Cierra la hoja y repite lo mismo con cada una de las tablas de la pestaña "Ventas" y "Categoría".

![img58](../images/img58.png)

Paso 4. Una vez que ya están todas las tablas en Power Pivot, cambia sus nombres al dar clic derecho en la opción "Cambiar nombre".

![img59](../images/img59.png)

Los nombre deben quedar de la siguiente manera: 

![img60](../images/img60.png)

Paso 5. Dirígete a la opción de "Vista de diagrama" en Power Pivot.

![img61](../images/img61.png)

Paso 6. Crea las relaciones de la siguiente manera: 
- Tabla empleados (código) va a unirse a tabla ventas (código).
- Tabla Ventas (categoría) va a unirse a tabla categoría (categoría).

![img62](../images/img62.png)

### Tarea 2. Crear una tabla dinámica.

Paso 1. En la barra superior, selecciona "Tabla dinámica".

![img63](../images/img63.png)

Paso 2. Selecciona una "Nueva hoja de cálculo".

![img64](../images/img64.png)

Paso 3. La tabla dinámica quedará en la columna del campo de "Nombre" que está en la tabla **Empleados**.

Las filas quedarán con el campo **Fecha** (de la tabla Ventas), **Categoría** (de la tabla Categoría) y **Productos** (de la tabla Ventas).

En valores, quedará la suma del campo total que está en la tabla "Ventas".

![img65](../images/img65.png)

Paso 4. Ve a la celda donde aparece la primera fecha (la cual es 04/05/2020), da clic derecho y selecciona "Agrupar".

![img66](../images/img66.png)

Selecciona la opción de "Meses" y "Aceptar".

![img67](../images/img67.png)

Paso 5. Selecciona una celda de la columna del "Total general", haz clic derecho y dirígete a "Formato número".

![img68](../images/img68.png)

Pao 6. Selecciona el formato moneda y las posiciones decimales: 0.

![img69](../images/img69.png)

### Tarea 3. Insertar segmentadores.

Paso 1. Posiciónate en la tabla dinámica y ve a la barra superior, en la opción de "Analizar tabla dinámica" selecciona "Insertar segmentación de datos".

![img70](../images/img70.png)

Paso 2. En la tabla "Categoría" selecciona la opción **Categoría**. Y, en la tabla "Ventas", selecciona **Productos**.

![img71](../images/img71.png)

![img72](../images/img72.png)

Paso 3. En los segmentadores insertados, selecciona "Consumo básico", "Azúcar" y "Café".

Paso 4. Guarda los cambios realizados y cierra el archivo.

> *Nota:* Si deseas, puedes cambiar el color de los segmentadores o de la tabla dinámica. Para esto, debes ir a la opción **Diseño**.

![img74](../images/img74.png)

![img75](../images/img75.png)

## Resultado esperado:

![img73](../images/img73.png)

---

# Práctica 3.3. Evaluación de ventas con KPIs en Power Pivot

## Objetivo de la práctica:
Al finalizar la práctica, serás capaz de:
- Integrar datos comerciales al modelo de Power Pivot.
- Crear una medida DAX que calculé el promedio de ventas por operación.
- Construir un KPI visual para evaluar el cumplimiento de metas de venta por producto.
- Analizar gráficamente los resultados mediante una tabla dinámica.

## Duración aproximada:
- 15 minutos.

## Escenario:
Trabajas en el área de inteligencia comercial de una empresa dedicada a la distribución de tecnología, mobiliario y telecomunicaciones a nivel nacional. Cada venta tiene un valor considerable, ya que se trata de productos empresariales.

La gerencia solicita un informe visual que indique qué productos están cumpliendo con el objetivo de ventas promedio por operación, fijado en $6,000 MXN.

Para ello, vas a construir un KPI con Power Pivot, el cual te permitirá visualizar este rendimiento con indicadores de color.

## Instrucciones:

### Tarea 1. Carga los datos al modelo de Power Pivot.

Paso 1. Descarga y abre el archivo [Práctica_módulo_3_ parte_3](práctica_módulo3_parte_3.xlsx).

Paso 2. Convierte los datos en una tabla (Crtl + T) y nómbrarla "VentasKPI".

![img76](../images/img76.png)

![img77](../images/img77.png)

Paso 3. Ve a la pestaña Power Pivot > Agregar al modelo de datos.

![img78](../images/img78.png)

### Tarea 2. Crear una medida de promedio de venta.

Paso 1. Da formato de moneda a la columna **Precio** y **Total**.

![img79](../images/img79.png)

Paso 2. En el "Área de cálculo", crea una medida con la siguiente fórmula:

![img80](../images/img80.png)

```
PromedioVenta := AVERAGE(VentasKPI[Total])
```

![img81](../images/img81.png)

Paso 3. Para dar formato al promedio de venta, haz clic derecho en la opción de "Formato" y selecciona Moneda, Simbolo $ y Posiciones decimales: 1.

![img82](../images/img82.png)


### Tarea 3. Crear el KPI.

Paso 1. Selecciona la medida de Promedio de Venta.

Paso 2. Haz clic en "Crear KPI" en la pestaña de **Inicio** de Power Pivot.

![img83](../images/img83.png)

Paso 3. Configura el KPI de la siguiente forma:

Valor objetivo absoluto: 6000

Indicadores de estado:

🔴 Rojo si < 4000

🟡 Amarillo si entre 4000 y 6000

🟢 Verde si > 6000

Paso 4. Confirma al dar clic en **Aceptar**.

![img84](../images/img84.png)

### Tarea 4. Crear una tabla dinámica para visualizar.

Paso 1. Regresa a la hoja de Excel en donde se encuentra la tabla y selecciona la opción de insertar "Tabla dinámica". Haz clic en la opción de "Desde modelo de datos" y "En una nueva hoja". 

![img85](../images/img85.png)

Paso 2. En la tabla dinámica:

- Agrega **Producto** a **Filas**.

- Agrega a Valores:
    - Promedio de venta.
    - Estado del KPI (el icono visual).

![img86](../images/img86.png)

Paso 3. Guarda los cambios y cierra el libro.

## Resultado esperado

![img87](../images/img87.png)
