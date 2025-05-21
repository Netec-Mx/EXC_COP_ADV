# Alerta por stock bajo en inventario con Power Automate

## Objetivo de la práctica:
Al finalizar la práctica, serás capaz de:
- Leer registros de una tabla de Excel desde OneDrive.
- Evaluar una condición basada en un valor numérico (Stock actual < Stock mínimo).
- Enviar una alerta personalizada al encargado de inventario.
- Formatear y presentar valores numéricos correctamente en el correo.


## Duración aproximada:
- 20 minutos.

## Escenario:
Formas parte del equipo de logística de una empresa.
Llevan el inventario en una tabla de Excel con columnas como producto, stock actual, y stock mínimo.
Tu objetivo es configurar un flujo que revise diariamente esa tabla y envíe una alerta automática si algún producto está por debajo del stock mínimo.

## Instrucciones 

### Tarea 1. Crear el archivo en Excel y subirlo a OneDrive

Paso 1. Genera la siguiente tabla de inventario en excel, ya sea en excel Online, o en tu máquina y subelo a OneDrive.

$Nota$ : En el correo del encargado, coloca tu correo ya que aquí se hará el envío de correo para está práctica.


ID| Producto	| Stock actual	| Stock mínimo	| Encargado

1| 	Laptops Dell| 	   8	        | 10            |mitzi.montiel@netec.com

2| 	Ratones   | 25	                | 20            |mitzi.montiel@netec.com

3| 	Cables HDMI| 4              | 10            |mitzi.montiel@netec.com

4| 	Memorias USB| 	16          | 8             |mitzi.montiel@netec.com

5| 	Sillas ergonomicas| 16      | 15            |mitzi.montiel@netec.com

6| 	Proyectores| 11	            |15	            |mitzi.montiel@netec.com

7| 	Cargadores universales| 7   |7              |mitzi.montiel@netec.com



Paso 2. Inserta el formato tabla

![img112](../images/img112.png)

Paso 3. Guarda el archivo como $Inventario$

![img113](../images/img113.png)



### Tarea 2. En Power Automate, crea un flujo programado

Paso 1. Ingresa a https://make.powerautomate.com 

Paso 2. Selecciona la opción "Flujo de nube programado"
![img114](../images/img114.png)

Paso 2. Añade un nombre como "Alerta por stock bajo"
Paso 3. La frecuencia escoje "Cada día"

![img115](../images/img115.png)


 ### Tarea 3. Agrega acción: “List rows present in a table”

 Paso 1. Da clic en el simbolo "+" para añadir una acción

 ![img116](../images/img116.png)

 Paso 2. Buscamos la opción "List rows present in a table"

  ![img117](../images/img117.png)

Paso 3: Llene los campos con la información
Ubicación: One Drive for Bussines
Biblioteca de documentos: Documentos
Archivo: Inventario.xlsx
Tabla: Tabla1 
  ![img118](../images/img118.png)

### Tarea 4. Agrega "Apply to each"

Paso 1. Da clic en insertar una acción en el cuadro de "Listar filas presentes en una tabla"

  ![img119](../images/img119.png)

Paso 2. Busca "Apply to each"

  ![img120](../images/img120.png)

Paso 3. Valor de entrada: "value" 

  ![img121](../images/img121.png)

Seleccionamor cuerpo/valor
  ![img122](../images/img122.png)



### Tarea 5. Agrega Una condición

Paso 1. Dentro del ciclo añadimos una acción

  ![img123](../images/img123.png)

Paso 2. Buscamos "Condition"

  ![img124](../images/img124.png)

Paso 3. En Choose a value, seleccionamos Stock actual

![img125](../images/img125.png)

Paso 4. Seleccionamos la opcion "is less than" y también seleccionamos "Stock mínimo"

![img126](../images/img126.png)

### Tarea 6. En el bloque “Sí”, agrega: Enviar un correo (V2)

Paso 1. En el bloque de "Si" agregamos una acción

![img127](../images/img127.png)

Paso 2. Buscamos la acción de "Send an email (V2)

![img128](../images/img128.png)

Paso 3. Llenamos los valores de la siguiente manera

Para: valor de la columna "Encargado"

![img129](../images/img129.png)

Subject: ⚠️ Stock bajo detectado 

$Body:$

Hola,

Se ha detectado un producto con stock bajo:

📦 Producto:   @{items('Apply_to_each')?['Producto']}
📉 Stock actual:   @{items('Apply_to_each')?['Stock actual']}
📊 Stock mínimo requerido: @{items('Apply_to_each')?['Stock mínimo']}

Por favor, programa reposición lo antes posible.

Gracias,  
Automatización con Power Automate

![img130](../images/img130.png)

### Tarea 7. Realizar prueba del flujo

Paso 1. Damos clic en "Save"
![img131](../images/img131.png)

Paso 2. Seleccionamos la opción Test y "Manually"

![img132](../images/img132.png)

![img133](../images/img133.png)

Paso 3. Damos clic en Run Flow

![img134](../images/img134.png)

Paso 4. Verás todo el flujo que corre de manera correcta.

![img135](../images/img135.png)


### Resultado esperado
Si el stock actual es menor que el mínimo, se enviará un correo de alerta.

El correo tendrá los datos del producto y niveles de inventario.

![img136](../images/img136.png)
