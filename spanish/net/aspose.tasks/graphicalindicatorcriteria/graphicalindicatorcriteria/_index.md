---
title: "GraphicalIndicatorCriteria.GraphicalIndicatorCriteria"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor de GraphicalIndicatorCriteria. Inicializa una nueva instancia del tipo GraphicalIndicatorCriteria"
type: docs
weight: 10
url: /es/net/aspose.tasks/graphicalindicatorcriteria/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) {#constructor_1}

Inicializa una nueva instancia del tipo [`GraphicalIndicatorCriteria`](../).

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value1, 
    GraphicalIndicatorCriteriaValue value2)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | valor del enum [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) que indica a qué filas se aplica el indicador |
| test | FilterComparisonType | valor de [`FilterComparisonType`](../../filtercomparisontype/) que denota el tipo de comparación realizado por el criterio. |
| imageIndex | Int32 | el índice de la imagen a mostrar cuando el campo cumple con los criterios |
| value1 | GraphicalIndicatorCriteriaValue | valores utilizados en la verificación de la condición. |
| value2 | GraphicalIndicatorCriteriaValue | segundo valor (fin del intervalo) utilizado en la verificación de la condición en caso de condiciones 'IsWithin' e 'IsNotWithing'. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | Se lanza cuando se pasa una combinación incorrecta de argumentos al constructor. |

### Ver también

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)

---

## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) {#constructor}

Inicializa una nueva instancia del tipo [`GraphicalIndicatorCriteria`](../).

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | valor del enum [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) que indica a qué filas se aplica el indicador |
| test | FilterComparisonType | valor de [`FilterComparisonType`](../../filtercomparisontype/) que denota el tipo de comparación realizado por el criterio. |
| imageIndex | Int32 | el índice de la imagen a mostrar cuando el campo cumple con los criterios |
| value | GraphicalIndicatorCriteriaValue | valor utilizado en la verificación de la condición. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | Se lanza cuando se pasa una combinación incorrecta de argumentos al constructor. |
| ArgumentException | Cuando el valor de IsWithin o IsNotWithing se pasa al argumento de prueba. |

### Ver también

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


