---
title: GraphicalIndicatorCriteria
second_title: Aspose.Tasks for Java API Reference
description: Represents one graphical indicator criteria associated with an extended attribute.
type: docs
weight: 114
url: /java/com.aspose.tasks/graphicalindicatorcriteria/
---

**Inheritance:**
java.lang.Object
```
public final class GraphicalIndicatorCriteria
```

Represents one graphical indicator criteria associated with an extended attribute.
## Constructors

| Constructor | Description |
| --- | --- |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | Initializes a new instance of the [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) type. |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | Initializes a new instance of the [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) type. |
## Methods

| Method | Description |
| --- | --- |
| [getImageIndex()](#getImageIndex--) | Gets the index of the image to display when the field meets the criteria. |
| [getRowType()](#getRowType--) | Gets the value of [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) enum which denotes for which rows the indicator is applied. |
| [getTest()](#getTest--) | Gets the type of comparison made between extended attribute's value and Values that acts as a criteria for the application of the graphical indicator. |
| [getValue1()](#getValue1--) | Gets the value used to test extended attribute's value. |
| [getValue2()](#getValue2--) | Gets the second value used to test extended attribute's value in case of 'IsWithin' and 'IsNotWithin' comparison types. |
| [toString()](#toString--) | Returns string representation of the instance of the [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) class. |
### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)
```


Initializes a new instance of the [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowType | int | value of [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) enum which denotes for which rows the indicator is applied |
| test | int | value of [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) denoting the type of comparison performed by the criteria. |
| imageIndex | int | the index of the image to display when the field meets the criteria |
| value1 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | values used in condition check. |
| value2 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | second value (end of interval) used in condition check in case of 'IsWithin' and 'IsNotWithing' conditions. |

### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```


Initializes a new instance of the [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowType | int | value of [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) enum which denotes for which rows the indicator is applied |
| test | int | value of [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) denoting the type of comparison performed by the criteria. |
| imageIndex | int | the index of the image to display when the field meets the criteria |
| value | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | value used in condition check. |

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


Gets the index of the image to display when the field meets the criteria.

**Returns:**
int - the index of the image to display when the field meets the criteria.
### getRowType() {#getRowType--}
```
public final int getRowType()
```


Gets the value of [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) enum which denotes for which rows the indicator is applied.

**Returns:**
int - the value of [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) enum which denotes for which rows the indicator is applied.
### getTest() {#getTest--}
```
public final int getTest()
```


Gets the type of comparison made between extended attribute's value and Values that acts as a criteria for the application of the graphical indicator. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - the type of comparison made between extended attribute's value and Values that acts as a criteria for the application of the graphical indicator.
### getValue1() {#getValue1--}
```
public final GraphicalIndicatorCriteriaValue getValue1()
```


Gets the value used to test extended attribute's value.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the value used to test extended attribute's value.
### getValue2() {#getValue2--}
```
public final GraphicalIndicatorCriteriaValue getValue2()
```


Gets the second value used to test extended attribute's value in case of 'IsWithin' and 'IsNotWithin' comparison types.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the second value used to test extended attribute's value in case of 'IsWithin' and 'IsNotWithin' comparison types.
### toString() {#toString--}
```
public String toString()
```


Returns string representation of the instance of the [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) class.

**Returns:**
java.lang.String - string representation of this object.
