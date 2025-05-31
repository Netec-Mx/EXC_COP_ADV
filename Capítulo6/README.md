# Práctica 6. Aplicación de DAX para análisis de ventas y servicio

## Objetivo de la práctica:
Al finalizar la práctica, serás capaz de:

- Aplicar funciones clave de DAX como CALCULATE, FILTER, DIVIDE y AVERAGEX para resolver necesidades de negocio relacionadas con el análisis de propinas por mesero y ventas por tipo de producto. El participante comprenderá cómo filtrar contextos y crear medidas relevantes para análisis operativos.

## Duración aproximada:
- 20 minutos.

---

**[⬅️ Atrás](https://netec-mx.github.io/EXC_COP_ADV/Cap%C3%ADtulo5/)** | **[Lista General](https://netec-mx.github.io/EXC_COP_ADV/)** | **[Siguiente ➡️](https://netec-mx.github.io/EXC_COP_ADV/Cap%C3%ADtulo7/)**

---

## Escenario: 

Trabajas en el área de análisis de un restaurante. El gerente general solicita un informe donde pueda ver:

- Cuánto ha recaudado cada mesero en propinas.
- Quién tiene mejor promedio de propina por pedido.
- Cuánto se ha vendido por tipo de producto (Comida vs Bebida).
- Cuánto se ha vendido exclusivamente en productos de comida con precio menor a $100.

## Instrucciones:

### Tarea 1. Cargar la base de datos de Excel a Power Pivot.

Paso 1. Descarga el archivo: [Practica Modulo 6](<Práctica Modulo 6.xlsx>).

Paso 2. Dirígete a la parte superior en Power Pivot y selecciona "Agregar a modelo de datos".

![img137](../images/img137.png)

![img138](../images/img138.png)

### Tarea 2. Crear las medidas DAX.

Paso 1. Posiciónate en el área de cálculo.

Paso 2. Para poder calcular el "Total de propinas por mesero", utiliza la siguiente fórmula:

```
TotalPropinas:=SUM(Restaurant[Propina])
```

Paso 3. Al cálculo realizado, asígnale el formato de **Moneda**.

![img139](../images/img139.png)

Paso 4. Para calcular el promedio de propina por pedido (orden), escribe la siguiente fórmula:

```
PromedioPropina:=AVERAGEX(
    VALUES(Restaurant[Orden]),
    CALCULATE(SUM(Restaurant[Propina]))
)
```

Paso 5. Al cálculo realizado, asígnale el formato de **Moneda**.

![img140](../images/img140.png)

Esto calcula el promedio por pedido (Orden), agrupando todos los registros con el mismo número de orden.

Paso 6. Calcula el **Total de ventas** por tipo de producto.

```
VentasTotales:=SUM(Restaurant[Precio])
```

Paso 7. Aplica el formato **Moneda**.

![img141](../images/img141.png)

Paso 8. Calcula las ventas de comida con precio menor a $100.

```
VentasComidaMenor100:=CALCULATE(
    [VentasTotales],
    FILTER(
        Restaurant,
        Restaurant[Tipo] = "Comida" &&
        Restaurant[Precio] < 100
    )
)
```

Paso 9. Aplica el formato **Moneda**.

![img142](../images/img142.png)

Filtra toda la tabla "Restaurant" para solo incluir productos tipo comida con precio menor a 100.

### Tarea 3. Realizar tablas dinámicas.

Paso 1. En la interfaz de Power Pivot, selecciona "Tabla dinámica" en una nueva hoja. 

![img143](../images/img143.png)

Paso 2. Realiza la primera tabla de las "Propinas por mesero".

- Filas ➡️ Restaurant[Atendió]
- Valores ➡️ Total Propinas

![img144](../images/img144.png)

Paso 3. Agrega el promedio por pedido (orden). Selecciona la medida de "PromedioPropina" para asignarla al campo valores.

![img145](../images/img145.png)

Paso 4. Copia y pega esa tabla dinámica, limpia todos los campos y, posteriormente, estructura las ventas por tipo.

- Filas ➡️ Restaurant[Tipo]
- Valores ➡️ VentasTotales

Se tiene que las ventas totales fueron de $2,051,629.

![img146](../images/img146.png)

Paso 5. Agrega a la tabla la medida que se realizó de **VentasComidaMenor100**.

![img147](../images/img147.png)

## Resultado esperado:

En el análisis realizado, se identificó que el total recaudado en propinas entre todos los meseros fue de $3,560.18, siendo Mauricio quien destacó significativamente con $551.20, la cifra más alta de forma individual. Además, al evaluar el promedio de propina por pedido, Mauricio nuevamente lidera con un promedio de $2.43, muy por encima del promedio general de $1.42, lo cual sugiere un desempeño destacado en atención al cliente o tipo de servicio brindado. En cuanto a las ventas por tipo de producto, se determinó que la comida generó $1,392,755, representando la mayor parte del ingreso frente a las bebidas con $658,874. Finalmente, se observó que dentro de las ventas de comida, los productos con precio menor a $100 representaron un volumen importante, alcanzando un total de $653,942, lo cual evidencia una alta demanda de opciones accesibles dentro del menú.

![img148](../images/img148.png)
