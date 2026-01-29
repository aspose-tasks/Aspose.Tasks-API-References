---
title: View
second_title: Aspose.Tasks for Java API Reference
description: Represents a view in Project.
type: docs
weight: 341
url: /java/com.aspose.tasks/view/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public class View implements Comparable<View>
```

Represents a view in Project.
## Constructors

| Constructor | Description |
| --- | --- |
| [View()](#View--) | Initializes a new instance of the [View](../../com.aspose.tasks/view) class. |
## Methods

| Method | Description |
| --- | --- |
| [compareTo(View other)](#compareTo-com.aspose.tasks.View-) | Compares the current instance with another object of the same type and returns an integer that indicates whether the current instance precedes, follows, or occurs in the same position in the sort order as the other object. |
| [equals(Object obj)](#equals-java.lang.Object-) | Returns a value indicating whether this instance is equal to a specified object. |
| [forViewScreen(int viewScreen)](#forViewScreen-int-) | Constructs a new instance of the [View](../../com.aspose.tasks/view) class. |
| [getFilter()](#getFilter--) | Gets a filter used in a single view. |
| [getGroup()](#getGroup--) | Gets a group of the single view. |
| [getHighlightFilter()](#getHighlightFilter--) | Gets a value indicating whether Microsoft Project highlights the filter for a single view. |
| [getName()](#getName--) | Gets the name of a View object. |
| [getPageInfo()](#getPageInfo--) | Gets an instance of the `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) class. |
| [getParentProject()](#getParentProject--) | Gets the parent of the View object. |
| [getScreen()](#getScreen--) | Gets the screen type for the single view. |
| [getShowInMenu()](#getShowInMenu--) | Gets a value indicating whether Microsoft Project shows the single view name in the View or the Other Views drop-down lists in the Ribbon. |
| [getTable()](#getTable--) | Gets a table of the single view. |
| [getType()](#getType--) | Gets the type of item in the single view, such as tasks or resources. |
| [getUid()](#getUid--) | Gets the unique identifier of a view. |
| [getVisualObjectsPlacements()](#getVisualObjectsPlacements--) | Gets a collection of objects representing placement and appearance of [OleObject](../../com.aspose.tasks/oleobject) in the view. |
| [hashCode()](#hashCode--) | Returns a hash code value for the instance of the [Resource](../../com.aspose.tasks/resource) class. |
| [op_Equality(View a, View b)](#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-) | Returns a value indicating whether this instance is equal to a specified object. |
| [op_GreaterThan(View a, View b)](#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-) | Returns a value indicating whether this instance is greater than a specified object. |
| [op_GreaterThanOrEqual(View a, View b)](#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | Returns a value indicating whether this instance is greater than or equal to a specified object. |
| [op_Inequality(View a, View b)](#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-) | Returns a value indicating whether this instance is not equal to a specified object. |
| [op_LessThan(View a, View b)](#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-) | Returns a value indicating whether this instance is less than a specified object. |
| [op_LessThanOrEqual(View a, View b)](#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | Returns a value indicating whether this instance is less than or equal to a specified object. |
| [setFilter(Filter value)](#setFilter-com.aspose.tasks.Filter-) | Sets a filter used in a single view. |
| [setGroup(Group value)](#setGroup-com.aspose.tasks.Group-) | Sets a group of the single view. |
| [setHighlightFilter(boolean value)](#setHighlightFilter-boolean-) | Sets a value indicating whether Microsoft Project highlights the filter for a single view. |
| [setName(String value)](#setName-java.lang.String-) | Sets the name of a View object. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Sets a value indicating whether Microsoft Project shows the single view name in the View or the Other Views drop-down lists in the Ribbon. |
| [setTable(Table value)](#setTable-com.aspose.tasks.Table-) | Sets a table of the single view. |
### View() {#View--}
```
public View()
```


Initializes a new instance of the [View](../../com.aspose.tasks/view) class.

### compareTo(View other) {#compareTo-com.aspose.tasks.View-}
```
public final int compareTo(View other)
```


Compares the current instance with another object of the same type and returns an integer that indicates whether the current instance precedes, follows, or occurs in the same position in the sort order as the other object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| other | [View](../../com.aspose.tasks/view) | the specified View object to compare this instance to. |

**Returns:**
int - A 32-bit signed integer that indicates the relative order of the objects being compared. The return value has these meanings: Value Meaning Less than zero This instance precedes `other` in the sort order. Zero This instance occurs in the same position in the sort order as `other`. Greater than zero This instance follows `other` in the sort order.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Returns a value indicating whether this instance is equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | The object to compare with this instance. |

**Returns:**
boolean - **True** if the specified object is a View that has the same Uid value as this instance; otherwise, **false**.
### forViewScreen(int viewScreen) {#forViewScreen-int-}
```
public static View forViewScreen(int viewScreen)
```


Constructs a new instance of the [View](../../com.aspose.tasks/view) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| viewScreen | int | The screen type for which the view can be displayed. |

**Returns:**
[View](../../com.aspose.tasks/view) - Constructed view.
### getFilter() {#getFilter--}
```
public final Filter getFilter()
```


Gets a filter used in a single view.

**Returns:**
[Filter](../../com.aspose.tasks/filter) - a filter used in a single view.
### getGroup() {#getGroup--}
```
public final Group getGroup()
```


Gets a group of the single view.

**Returns:**
[Group](../../com.aspose.tasks/group) - a group of the single view.
### getHighlightFilter() {#getHighlightFilter--}
```
public final boolean getHighlightFilter()
```


Gets a value indicating whether Microsoft Project highlights the filter for a single view.

**Returns:**
boolean - a value indicating whether Microsoft Project highlights the filter for a single view.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of a View object.

**Returns:**
java.lang.String - the name of a View object.
### getPageInfo() {#getPageInfo--}
```
public final PageInfo getPageInfo()
```


Gets an instance of the `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) class. Represents page setup data which is present in mpp file format.

**Returns:**
[PageInfo](../../com.aspose.tasks/pageinfo) - an instance of the `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) class.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Gets the parent of the View object. Read-only [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### getScreen() {#getScreen--}
```
public final int getScreen()
```


Gets the screen type for the single view. Read-only [ViewScreen](../../com.aspose.tasks/viewscreen).

**Returns:**
int - the screen type for the single view.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Gets a value indicating whether Microsoft Project shows the single view name in the View or the Other Views drop-down lists in the Ribbon.

**Returns:**
boolean - a value indicating whether Microsoft Project shows the single view name in the View or the Other Views drop-down lists in the Ribbon.
### getTable() {#getTable--}
```
public final Table getTable()
```


Gets a table of the single view.

**Returns:**
[Table](../../com.aspose.tasks/table) - a table of the single view.
### getType() {#getType--}
```
public final int getType()
```


Gets the type of item in the single view, such as tasks or resources. Read-only [ItemType](../../com.aspose.tasks/itemtype).

**Returns:**
int - the type of item in the single view, such as tasks or resources.
### getUid() {#getUid--}
```
public final int getUid()
```


Gets the unique identifier of a view.

**Returns:**
int - the unique identifier of a view.
### getVisualObjectsPlacements() {#getVisualObjectsPlacements--}
```
public final List<VisualObjectPlacement> getVisualObjectsPlacements()
```


Gets a collection of objects representing placement and appearance of [OleObject](../../com.aspose.tasks/oleobject) in the view.

**Returns:**
java.util.List&lt;com.aspose.tasks.VisualObjectPlacement&gt; - a collection of objects representing placement and appearance of [OleObject](../../com.aspose.tasks/oleobject) in the view.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returns a hash code value for the instance of the [Resource](../../com.aspose.tasks/resource) class.

**Returns:**
int - returns a hash code value for this object.
### op_Equality(View a, View b) {#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Equality(View a, View b)
```


Returns a value indicating whether this instance is equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | The first view. |
| b | [View](../../com.aspose.tasks/view) | The second view. |

**Returns:**
boolean - a value indicating whether this instance is equal to a specified object
### op_GreaterThan(View a, View b) {#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThan(View a, View b)
```


Returns a value indicating whether this instance is greater than a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | The first view. |
| b | [View](../../com.aspose.tasks/view) | The second view. |

**Returns:**
boolean - a value indicating whether this instance is greater than a specified object
### op_GreaterThanOrEqual(View a, View b) {#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThanOrEqual(View a, View b)
```


Returns a value indicating whether this instance is greater than or equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | The first view. |
| b | [View](../../com.aspose.tasks/view) | The second view. |

**Returns:**
boolean - a value indicating whether this instance is greater than or equal to a specified object
### op_Inequality(View a, View b) {#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Inequality(View a, View b)
```


Returns a value indicating whether this instance is not equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | The first view. |
| b | [View](../../com.aspose.tasks/view) | The second view. |

**Returns:**
boolean - a value indicating whether this instance is not equal to a specified object
### op_LessThan(View a, View b) {#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThan(View a, View b)
```


Returns a value indicating whether this instance is less than a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | The first filter. |
| b | [View](../../com.aspose.tasks/view) | The second filter. |

**Returns:**
boolean - a value indicating whether this instance is less than a specified object
### op_LessThanOrEqual(View a, View b) {#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThanOrEqual(View a, View b)
```


Returns a value indicating whether this instance is less than or equal to a specified object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | The first view. |
| b | [View](../../com.aspose.tasks/view) | The second view. |

**Returns:**
boolean - a value indicating whether this instance is less than or equal to a specified object
### setFilter(Filter value) {#setFilter-com.aspose.tasks.Filter-}
```
public final void setFilter(Filter value)
```


Sets a filter used in a single view.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Filter](../../com.aspose.tasks/filter) | a filter used in a single view. |

### setGroup(Group value) {#setGroup-com.aspose.tasks.Group-}
```
public final void setGroup(Group value)
```


Sets a group of the single view.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Group](../../com.aspose.tasks/group) | a group of the single view. |

### setHighlightFilter(boolean value) {#setHighlightFilter-boolean-}
```
public final void setHighlightFilter(boolean value)
```


Sets a value indicating whether Microsoft Project highlights the filter for a single view.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether Microsoft Project highlights the filter for a single view. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets the name of a View object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the name of a View object. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Sets a value indicating whether Microsoft Project shows the single view name in the View or the Other Views drop-down lists in the Ribbon.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether Microsoft Project shows the single view name in the View or the Other Views drop-down lists in the Ribbon. |

### setTable(Table value) {#setTable-com.aspose.tasks.Table-}
```
public final void setTable(Table value)
```


Sets a table of the single view.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Table](../../com.aspose.tasks/table) | a table of the single view. |

