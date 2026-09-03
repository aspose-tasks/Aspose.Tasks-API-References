---
title: "Aspose::Tasks::GraphicalIndicatorCriteria::GraphicalIndicatorCriteria constructor"
linktitle: "GraphicalIndicatorCriteria"
articleTitle: "GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for C++"
description: "Inicializa una nueva instancia del tipo GraphicalIndicatorCriteria."
type: docs
weight: 10
url: /es/cpp/aspose.tasks/graphicalindicatorcriteria/graphicalindicatorcriteria/
---

## GraphicalIndicatorCriteria (1 of 2) {#graphicalindicatorcriteria_1}

Inicializa una nueva instancia del tipo GraphicalIndicatorCriteria.

**Returns:** Aspose::Tasks::

```cpp
GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, FilterComparisonType test, int32_t imageIndex, const System::SharedPtr< GraphicalIndicatorCriteriaValue > & value1, const System::SharedPtr< GraphicalIndicatorCriteriaValue > & value2)
```

| Parámetro | Descripción |
| --- | --- |
| rowType | valor del enum GraphicalIndicatorCriteriaType que indica para qué filas se aplica el indicador |
| prueba | valor de FilterComparisonType que indica el tipo de comparación realizada por el criterio. |
| imageIndex | el índice de la imagen a mostrar cuando el campo cumple los criterios |
| value1 | valores utilizados en la verificación de la condición. |
| value2 | segundo valor (fin del intervalo) utilizado en la verificación de la condición en caso de condiciones 'IsWithin' y 'IsNotWithing'. |

---

## GraphicalIndicatorCriteria (2 of 2) {#graphicalindicatorcriteria_2}

Inicializa una nueva instancia del tipo GraphicalIndicatorCriteria.

**Returns:** Aspose::Tasks::

```cpp
GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, FilterComparisonType test, int32_t imageIndex, const System::SharedPtr< GraphicalIndicatorCriteriaValue > & value)
```

| Parámetro | Descripción |
| --- | --- |
| rowType | valor del enum GraphicalIndicatorCriteriaType que indica para qué filas se aplica el indicador |
| prueba | valor de FilterComparisonType que indica el tipo de comparación realizada por el criterio. |
| imageIndex | el índice de la imagen a mostrar cuando el campo cumple los criterios |
| valor | valor utilizado en la verificación de la condición. |

