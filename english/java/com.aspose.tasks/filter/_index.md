---
title: Filter
second_title: Aspose.Tasks for Java API Reference
description: Represents a filter in Project.
type: docs
weight: 91
url: /java/com.aspose.tasks/filter/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public final class Filter implements Comparable<Filter>, System.IEquatable<Filter>
```

Represents a filter in Project.
## Constructors

| Constructor | Description |
| --- | --- |
| [Filter()](#Filter--) |  |
## Methods

| Method | Description |
| --- | --- |
| [compareTo(Filter other)](#compareTo-com.aspose.tasks.Filter-) | Compares this instance to the specified instance of the [Filter](../../com.aspose.tasks/filter) class and returns an indication of their relative order. |
| [equals(Filter other)](#equals-com.aspose.tasks.Filter-) | Returns a value indicating whether this instance is equal to the specified AssignmentBaseline object. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returns a value indicating whether this instance is equal to the specified AssignmentBaseline object. |
| [getCriteria()](#getCriteria--) | Gets the criteria that tasks or resources must meet to be displayed in MSP view. |
| [getFilterType()](#getFilterType--) | Gets the type of the filter. |
| [getIndex()](#getIndex--) | Gets the index of a [Filter](../../com.aspose.tasks/filter) object in the Filters containing object. |
| [getName()](#getName--) | Gets the name of a Filter object. |
| [getParentProject()](#getParentProject--) | Gets the parent of the Filter object. |
| [getShowInMenu()](#getShowInMenu--) | Gets a value indicating whether project shows the filter name in the Filter drop-down list on the View tab of the Ribbon. |
| [getShowRelatedSummaryRows()](#getShowRelatedSummaryRows--) | Gets a value indicating whether related summary rows are displayed for the filter. |
| [getUid()](#getUid--) | Gets the unique identifier of a filter. |
| [hashCode()](#hashCode--) | Returns a hash code value for the filter. |
| [op_Equality(Filter a, Filter b)](#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Returns a value indicating whether this instance is equal to a specified object. |
| [op_GreaterThan(Filter a, Filter b)](#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Returns a value indicating whether this instance is greater than a specified object. |
| [op_GreaterThanOrEqual(Filter a, Filter b)](#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Returns a value indicating whether this instance is greater than or equal to a specified object. |
| [op_Inequality(Filter a, Filter b)](#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Returns a value indicating whether this instance is not equal to a specified object. |
| [op_LessThan(Filter a, Filter b)](#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Returns a value indicating whether this instance is less than a specified object. |
| [op_LessThanOrEqual(Filter a, Filter b)](#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Returns a value indicating whether this instance is less than or equal to a specified object. |
| [setCriteria(FilterCriteria value)](#setCriteria-com.aspose.tasks.FilterCriteria-) | Sets the criteria that tasks or resources must meet to be displayed in MSP view. |
| [setName(String value)](#setName-java.lang.String-) | Sets the name of a Filter object. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Sets a value indicating whether project shows the filter name in the Filter drop-down list on the View tab of the Ribbon. |
| [setShowRelatedSummaryRows(boolean value)](#setShowRelatedSummaryRows-boolean-) | Sets a value indicating whether related summary rows are displayed for the filter. |
### Filter() {#Filter--}
```
public Filter()
```


### compareTo(Filter other) {#compareTo-com.aspose.tasks.Filter-}
```
public final int compareTo(Filter other)
```


Compares this instance to the specified instance of the [Filter](../../com.aspose.tasks/filter) class and returns an indication of their relative order.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | the specified instance of the [Filter](../../com.aspose.tasks/filter) class to compare to this object. |

**Returns:**
int - an indication of their relative order.
### equals(Filter other) {#equals-com.aspose.tasks.Filter-}
```
public final boolean equals(Filter other)
```


Returns a value indicating whether this instance is equal to the specified AssignmentBaseline object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | the specified AssignmentBaseline object to compare with this instance. |

**Returns:**
boolean - returns true if this instance is equal to the specified AssignmentBaseline object; otherwise, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Returns a value indicating whether this instance is equal to the specified AssignmentBaseline object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | the specified AssignmentBaseline object to compare with this instance. |

**Returns:**
boolean - returns true if this instance is equal to the specified AssignmentBaseline object; otherwise, false.
### getCriteria() {#getCriteria--}
```
public final FilterCriteria getCriteria()
```


Gets the criteria that tasks or resources must meet to be displayed in MSP view.

**Returns:**
[FilterCriteria](../../com.aspose.tasks/filtercriteria) - the criteria that tasks or resources must meet to be displayed in MSP view.
### getFilterType() {#getFilterType--}
```
public final int getFilterType()
```


Gets the type of the filter.

**Returns:**
int - the type of the filter.
### getIndex() {#getIndex--}
```
public final int getIndex()
```


Gets the index of a [Filter](../../com.aspose.tasks/filter) object in the Filters containing object.

**Returns:**
int - the index of a [Filter](../../com.aspose.tasks/filter) object in the Filters containing object.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of a Filter object.

**Returns:**
java.lang.String - the name of a Filter object.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Gets the parent of the Filter object.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the Filter object.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Gets a value indicating whether project shows the filter name in the Filter drop-down list on the View tab of the Ribbon.

**Returns:**
boolean - a value indicating whether project shows the filter name in the Filter drop-down list on the View tab of the Ribbon.
### getShowRelatedSummaryRows() {#getShowRelatedSummaryRows--}
```
public final boolean getShowRelatedSummaryRows()
```


Gets a value indicating whether related summary rows are displayed for the filter.

**Returns:**
boolean - a value indicating whether related summary rows are displayed for the filter.
### getUid() {#getUid--}
```
public final int getUid()
```


Gets the unique identifier of a filter.

**Returns:**
int - the unique identifier of a filter.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returns a hash code value for the filter.

**Returns:**
int - returns a hash code value for this object.
### op_Equality(Filter a, Filter b) {#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Equality(Filter a, Filter b)
```


Returns a value indicating whether this instance is equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | The first filter. |
| b | [Filter](../../com.aspose.tasks/filter) | The second filter. |

**Returns:**
boolean - a value indicating whether this instance is equal to a specified object
### op_GreaterThan(Filter a, Filter b) {#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThan(Filter a, Filter b)
```


Returns a value indicating whether this instance is greater than a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | The first filter. |
| b | [Filter](../../com.aspose.tasks/filter) | The second filter. |

**Returns:**
boolean - a value indicating whether this instance is greater than a specified object
### op_GreaterThanOrEqual(Filter a, Filter b) {#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThanOrEqual(Filter a, Filter b)
```


Returns a value indicating whether this instance is greater than or equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | The first filter. |
| b | [Filter](../../com.aspose.tasks/filter) | The second filter. |

**Returns:**
boolean - a value indicating whether this instance is greater than or equal to a specified object
### op_Inequality(Filter a, Filter b) {#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Inequality(Filter a, Filter b)
```


Returns a value indicating whether this instance is not equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | The first filter. |
| b | [Filter](../../com.aspose.tasks/filter) | The second filter. |

**Returns:**
boolean - a value indicating whether this instance is not equal to a specified object
### op_LessThan(Filter a, Filter b) {#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThan(Filter a, Filter b)
```


Returns a value indicating whether this instance is less than a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | The first filter. |
| b | [Filter](../../com.aspose.tasks/filter) | The second filter. |

**Returns:**
boolean - a value indicating whether this instance is less than a specified object
### op_LessThanOrEqual(Filter a, Filter b) {#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThanOrEqual(Filter a, Filter b)
```


Returns a value indicating whether this instance is less than or equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | The first filter. |
| b | [Filter](../../com.aspose.tasks/filter) | The second filter. |

**Returns:**
boolean - a value indicating whether this instance is less than or equal to a specified object
### setCriteria(FilterCriteria value) {#setCriteria-com.aspose.tasks.FilterCriteria-}
```
public final void setCriteria(FilterCriteria value)
```


Sets the criteria that tasks or resources must meet to be displayed in MSP view.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FilterCriteria](../../com.aspose.tasks/filtercriteria) | the criteria that tasks or resources must meet to be displayed in MSP view. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets the name of a Filter object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the name of a Filter object. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Sets a value indicating whether project shows the filter name in the Filter drop-down list on the View tab of the Ribbon.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether project shows the filter name in the Filter drop-down list on the View tab of the Ribbon. |

### setShowRelatedSummaryRows(boolean value) {#setShowRelatedSummaryRows-boolean-}
```
public final void setShowRelatedSummaryRows(boolean value)
```


Sets a value indicating whether related summary rows are displayed for the filter.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether related summary rows are displayed for the filter. |

