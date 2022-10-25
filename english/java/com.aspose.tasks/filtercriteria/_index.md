---
title: FilterCriteria
second_title: Aspose.Tasks for Java API Reference
description: Defines the criteria that tasks or resources must meet to be displayed in MSP view.
type: docs
weight: 94
url: /java/com.aspose.tasks/filtercriteria/
---

**Inheritance:**
java.lang.Object
```
public class FilterCriteria
```

Defines the criteria that tasks or resources must meet to be displayed in MSP view.
## Constructors

| Constructor | Description |
| --- | --- |
| [FilterCriteria()](#FilterCriteria--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getCriteriaRows()](#getCriteriaRows--) | Gets the list of child [FilterCriteria](../../com.aspose.tasks/filtercriteria) rows. |
| [getField()](#getField--) | Gets a  Field ([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) to change. |
| [setField(int value)](#setField-int-) | Sets a  Field ([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) to change. |
| [getOperation()](#getOperation--) | Gets the criterion established with FieldName, Test, and Value relates to other criteria in the filter. |
| [setOperation(int value)](#setOperation-int-) | Sets the criterion established with FieldName, Test, and Value relates to other criteria in the filter. |
| [getTest()](#getTest--) | Gets the type of comparison made between FieldName and Value that acts as selection criteria for the filter. |
| [setTest(int value)](#setTest-int-) | Sets the type of comparison made between FieldName and Value that acts as selection criteria for the filter. |
| [getValues()](#getValues--) | Gets the object values to compare with the value of the field specified with FieldName. |
| [toString()](#toString--) | Returns string representation of the instance of the [FilterCriteria](../../com.aspose.tasks/filtercriteria) class. |
### FilterCriteria() {#FilterCriteria--}
```
public FilterCriteria()
```


### getCriteriaRows() {#getCriteriaRows--}
```
public final List<FilterCriteria> getCriteriaRows()
```


Gets the list of child [FilterCriteria](../../com.aspose.tasks/filtercriteria) rows. If the filter contains more than one criterion row then the effect of an And operator is that the criteria for both rows must be met for the task or resource to be displayed as a result of this filter. The effect of an Or operator is that the criteria for one or the other row must be met.

**Returns:**
java.util.List&lt;com.aspose.tasks.FilterCriteria&gt; - the list of child [FilterCriteria](../../com.aspose.tasks/filtercriteria) rows.
### getField() {#getField--}
```
public final int getField()
```


Gets a  Field ([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) to change.

**Returns:**
int - a  Field ([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) to change.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Sets a  Field ([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) to change.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a  Field ([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) to change. |

### getOperation() {#getOperation--}
```
public final int getOperation()
```


Gets the criterion established with FieldName, Test, and Value relates to other criteria in the filter.

**Returns:**
int - the criterion established with FieldName, Test, and Value relates to other criteria in the filter.
### setOperation(int value) {#setOperation-int-}
```
public final void setOperation(int value)
```


Sets the criterion established with FieldName, Test, and Value relates to other criteria in the filter.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the criterion established with FieldName, Test, and Value relates to other criteria in the filter. |

### getTest() {#getTest--}
```
public final int getTest()
```


Gets the type of comparison made between FieldName and Value that acts as selection criteria for the filter. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - the type of comparison made between FieldName and Value that acts as selection criteria for the filter.
### setTest(int value) {#setTest-int-}
```
public final void setTest(int value)
```


Sets the type of comparison made between FieldName and Value that acts as selection criteria for the filter. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the type of comparison made between FieldName and Value that acts as selection criteria for the filter. |

### getValues() {#getValues--}
```
public final Object[] getValues()
```


Gets the object values to compare with the value of the field specified with FieldName.

**Returns:**
java.lang.Object[] - the object values to compare with the value of the field specified with FieldName.
### toString() {#toString--}
```
public String toString()
```


Returns string representation of the instance of the [FilterCriteria](../../com.aspose.tasks/filtercriteria) class.

**Returns:**
java.lang.String - string representation of this object.
