---
title: GraphicalIndicatorCriteria.GraphicalIndicatorCriteria
second_title: Aspose.Tasks for .NET API Reference
description: GraphicalIndicatorCriteria constructor. Initializes a new instance of the GraphicalIndicatorCriteria type
type: docs
weight: 10
url: /net/aspose.tasks/graphicalindicatorcriteria/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) {#constructor_1}

Initializes a new instance of the [`GraphicalIndicatorCriteria`](../) type.

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value1, 
    GraphicalIndicatorCriteriaValue value2)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | value of [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) enum which denotes for which rows the indicator is applied |
| test | FilterComparisonType | value of [`FilterComparisonType`](../../filtercomparisontype/) denoting the type of comparison performed by the criteria. |
| imageIndex | Int32 | the index of the image to display when the field meets the criteria |
| value1 | GraphicalIndicatorCriteriaValue | values used in condition check. |
| value2 | GraphicalIndicatorCriteriaValue | second value (end of interval) used in condition check in case of 'IsWithin' and 'IsNotWithing' conditions. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Thrown when incorrect combination of arguments is passed to the constructor. |

### See Also

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)

---

## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) {#constructor}

Initializes a new instance of the [`GraphicalIndicatorCriteria`](../) type.

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | value of [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) enum which denotes for which rows the indicator is applied |
| test | FilterComparisonType | value of [`FilterComparisonType`](../../filtercomparisontype/) denoting the type of comparison performed by the criteria. |
| imageIndex | Int32 | the index of the image to display when the field meets the criteria |
| value | GraphicalIndicatorCriteriaValue | value used in condition check. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Thrown when incorrect combination of arguments is passed to the constructor. |
| ArgumentException | When value of IsWithin of IsNotWithing is passed to test argument. |

### See Also

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


