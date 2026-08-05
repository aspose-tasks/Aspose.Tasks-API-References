---
title: "Aspose::Tasks::GraphicalIndicatorCriteria::GraphicalIndicatorCriteria constructor"
linktitle: "GraphicalIndicatorCriteria"
articleTitle: "GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for C++"
description: "Initializes a new instance of the GraphicalIndicatorCriteria type."
type: docs
weight: 10
url: /cpp/aspose.tasks/graphicalindicatorcriteria/graphicalindicatorcriteria/
---

## GraphicalIndicatorCriteria (1 of 2) {#graphicalindicatorcriteria_1}

Initializes a new instance of the GraphicalIndicatorCriteria type.

**Returns:** Aspose::Tasks::

```cpp
GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, FilterComparisonType test, int32_t imageIndex, const System::SharedPtr< GraphicalIndicatorCriteriaValue > & value1, const System::SharedPtr< GraphicalIndicatorCriteriaValue > & value2)
```

| Parameter | Description |
| --- | --- |
| rowType | value of GraphicalIndicatorCriteriaType enum which denotes for which rows the indicator is applied |
| test | value of FilterComparisonType denoting the type of comparison performed by the criteria. |
| imageIndex | the index of the image to display when the field meets the criteria |
| value1 | values used in condition check. |
| value2 | second value (end of interval) used in condition check in case of 'IsWithin' and 'IsNotWithing' conditions. |

---

## GraphicalIndicatorCriteria (2 of 2) {#graphicalindicatorcriteria_2}

Initializes a new instance of the GraphicalIndicatorCriteria type.

**Returns:** Aspose::Tasks::

```cpp
GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, FilterComparisonType test, int32_t imageIndex, const System::SharedPtr< GraphicalIndicatorCriteriaValue > & value)
```

| Parameter | Description |
| --- | --- |
| rowType | value of GraphicalIndicatorCriteriaType enum which denotes for which rows the indicator is applied |
| test | value of FilterComparisonType denoting the type of comparison performed by the criteria. |
| imageIndex | the index of the image to display when the field meets the criteria |
| value | value used in condition check. |

