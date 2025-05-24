# Práctica 1. Control de acceso y protección de datos en un informe financiero

## Objetivo de la práctica:
Al finalizar la práctica, serás capaz de:
- Aplicar la protección de celdas específicas para evitar modificaciones no deseadas.
- Configurar contraseñas para restringir la apertura y edición del archivo.
- Bloquear la estructura del libro para impedir la manipulación de hojas.
- Ocultar fórmulas críticas que contienen cálculos financieros.
- Permitir la edición únicamente en las celdas designadas para entrada de datos.

## Duración aproximada:
- 15 minutos.

---

**[Lista General](https://netec-mx.github.io/EXC_COP_ADV/)** | **[Siguiente ➡️](https://netec-mx.github.io/EXC_COP_ADV/Cap%C3%ADtulo2/)**

---

## Instrucciones:

### Tarea 1. Preparar las celdas editables (comentarios)

Paso 1. Abrir el archivo llamado [Informe financiero 2024](<Informe financiero 2024.xlsx>). 

Seleccionar el rango $E2:E14$

![img1](../images/img1.png)

Paso 2. Hacer clic derecho en → Formato de celdas → Proteger → desmarca "Bloqueada".

![img2](../images/img2.png)

Paso 3. Esto permite que solo esa columna sea editable.


### Tarea 2. Ocultar las fórmulas

Paso 1. Seleccionar las celdas con fórmulas: columna D y fila 14 (D2:D14, B14:D14).

![img3](../images/img3.png)

Paso 2. Ir a Inicio → Formato de celdas → Protección → Marca "Oculta".

![img4](../images/img4.png)

![img5](../images/img5.png)


### Tarea 3. Activar la protección de hoja

Paso 1. Ir a Revisar → Proteger hoja.

Paso 2. Marcar solo “Seleccionar celdas desbloqueadas”.

Paso 3. Contraseña: Resumen2024

![img6](../images/img6.png)


### Tarea 4.  Proteger el libro (estructura)

Paso 1. Ir a Revisar → Proteger libro.

Paso 2. Marcar “Estructura” y asignar la contraseña: EstructuraFin

### Tarea 5. Proteger con contraseña el archivo

Paso 1. Ir a Archivo → Información → Proteger libro → Cifrar con contraseña.

Paso 2. Contraseña: Finanzas2024

![img7](../images/img7.png)

### Tarea 6. Proteger con contraseña el archivo

Paso 1. Ir a Archivo → Información → Proteger libro → Cifrar con contraseña.

![img8](../images/img8.png)

Paso 2. Contraseña: Finanzas2024

![img9](../images/img9.png)

Paso 3. Guardar los cambios y cerrar el archivo.

Paso 4. Abrir el archivo, ingresar la contraseña y colocar un comentario en la columna "Comentarios del analista".

### Resultado esperado
- Solo se podrán ingresar comentarios en la columna “Comentarios del analista”.

- Las fórmulas estarán ocultas y protegidas.

- No se podrán insertar, eliminar o mover hojas.

- El archivo completo no podrá abrirse o editarse sin contraseña.
![img10](../images/img10.png)

