---
title: "GraphicalIndicatorCriteria"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un criterio de indicador gráfico asociado a un atributo extendido."
type: docs
weight: 115
url: /es/java/com.aspose.tasks/graphicalindicatorcriteria/
---

**Inheritance:**
java.lang.Object
```
public final class GraphicalIndicatorCriteria
```

Representa un criterio de indicador gráfico asociado a un atributo extendido.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | Inicializa una nueva instancia del tipo [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria). |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | Inicializa una nueva instancia del tipo [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getImageIndex()](#getImageIndex--) | Obtiene el índice de la imagen que se mostrará cuando el campo cumpla los criterios. |
| [getRowType()](#getRowType--) | Obtiene el valor del enum [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) que indica para qué filas se aplica el indicador. |
| [getTest()](#getTest--) | Obtiene el tipo de comparación realizado entre el valor del atributo extendido y los Valores que actúan como criterio para la aplicación del indicador gráfico. |
| [getValue1()](#getValue1--) | Obtiene el valor utilizado para probar el valor del atributo extendido. |
| [getValue2()](#getValue2--) | Obtiene el segundo valor utilizado para probar el valor del atributo extendido en caso de los tipos de comparación 'IsWithin' y 'IsNotWithin'. |
| [toString()](#toString--) | Devuelve la representación en cadena de la instancia de la clase [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria). |
### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)
```


Inicializa una nueva instancia del tipo [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowType | int | valor del enum [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) que indica para qué filas se aplica el indicador |
| test | int | valor del [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) que indica el tipo de comparación realizado por el criterio. |
| imageIndex | int | el índice de la imagen que se mostrará cuando el campo cumpla los criterios |
| value1 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | valores utilizados en la comprobación de condición. |
| value2 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | segundo valor (fin del intervalo) utilizado en la comprobación de condición en caso de condiciones 'IsWithin' y 'IsNotWithing'. |

### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```


Inicializa una nueva instancia del tipo [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowType | int | valor del enum [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) que indica para qué filas se aplica el indicador |
| test | int | valor del [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) que indica el tipo de comparación realizado por el criterio. |
| imageIndex | int | el índice de la imagen que se mostrará cuando el campo cumpla los criterios |
| value | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | valor utilizado en la comprobación de condición. |

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


Obtiene el índice de la imagen que se mostrará cuando el campo cumpla los criterios.

**Returns:**
int - el índice de la imagen que se mostrará cuando el campo cumpla los criterios.
### getRowType() {#getRowType--}
```
public final int getRowType()
```


Obtiene el valor del enum [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) que indica para qué filas se aplica el indicador.

**Returns:**
int - el valor del enum [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) que indica para qué filas se aplica el indicador.
### getTest() {#getTest--}
```
public final int getTest()
```


Obtiene el tipo de comparación realizado entre el valor del atributo extendido y los Valores que actúan como criterio para la aplicación del indicador gráfico. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - el tipo de comparación realizado entre el valor del atributo extendido y los Valores que actúan como criterio para la aplicación del indicador gráfico.
### getValue1() {#getValue1--}
```
public final GraphicalIndicatorCriteriaValue getValue1()
```


Obtiene el valor utilizado para probar el valor del atributo extendido.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the value used to test extended attribute's value.
### getValue2() {#getValue2--}
```
public final GraphicalIndicatorCriteriaValue getValue2()
```


Obtiene el segundo valor utilizado para probar el valor del atributo extendido en caso de los tipos de comparación 'IsWithin' y 'IsNotWithin'.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the second value used to test extended attribute's value in case of 'IsWithin' and 'IsNotWithin' comparison types.
### toString() {#toString--}
```
public String toString()
```


Devuelve la representación en cadena de la instancia de la clase [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria).

**Returns:**
java.lang.String - representación en cadena de este objeto.
