---
title: "视图"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示 Project 中的视图。"
type: docs
weight: 342
url: /zh/java/com.aspose.tasks/view/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public class View implements Comparable<View>
```

表示 Project 中的视图。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [View()](#View--) | 初始化一个新的 [View](../../com.aspose.tasks/view) 类实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [compareTo(View other)](#compareTo-com.aspose.tasks.View-) | 比较当前实例与同类型的另一个对象，并返回一个整数，指示当前实例在排序顺序中是位于该对象之前、之后，还是与其处于相同位置。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [forViewScreen(int viewScreen)](#forViewScreen-int-) | 构造一个新的 [View](../../com.aspose.tasks/view) 类实例。 |
| [getFilter()](#getFilter--) | 获取在单个视图中使用的筛选器。 |
| [getGroup()](#getGroup--) | 获取单个视图的组。 |
| [getHighlightFilter()](#getHighlightFilter--) | 获取一个值，指示 Microsoft Project 是否突出显示单个视图的筛选器。 |
| [getName()](#getName--) | 获取 View 对象的名称。 |
| [getPageInfo()](#getPageInfo--) | 获取 `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\\#getPageInfo--)) 类的实例。 |
| [getParentProject()](#getParentProject--) | 获取 View 对象的父对象。 |
| [getScreen()](#getScreen--) | 获取单个视图的屏幕类型。 |
| [getShowInMenu()](#getShowInMenu--) | 获取一个值，指示 Microsoft Project 是否在功能区的 View 或 Other Views 下拉列表中显示单个视图的名称。 |
| [getTable()](#getTable--) | 获取单个视图的表格。 |
| [getType()](#getType--) | 获取单个视图中项目的类型，例如任务或资源。 |
| [getUid()](#getUid--) | 获取视图的唯一标识符。 |
| [getVisualObjectsPlacements()](#getVisualObjectsPlacements--) | 获取表示视图中 [OleObject](../../com.aspose.tasks/oleobject) 的放置和外观的对象集合。 |
| [hashCode()](#hashCode--) | 返回 [Resource](../../com.aspose.tasks/resource) 类实例的哈希码值。 |
| [op_Equality(View a, View b)](#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [op_GreaterThan(View a, View b)](#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-) | 返回一个值，指示此实例是否大于指定的对象。 |
| [op_GreaterThanOrEqual(View a, View b)](#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | 返回一个值，指示此实例是否大于或等于指定的对象。 |
| [op_Inequality(View a, View b)](#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-) | 返回一个值，指示此实例是否不等于指定的对象。 |
| [op_LessThan(View a, View b)](#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-) | 返回一个值，指示此实例是否小于指定的对象。 |
| [op_LessThanOrEqual(View a, View b)](#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-) | 返回一个值，指示此实例是否小于或等于指定的对象。 |
| [setFilter(Filter value)](#setFilter-com.aspose.tasks.Filter-) | 设置在单个视图中使用的筛选器。 |
| [setGroup(Group value)](#setGroup-com.aspose.tasks.Group-) | 设置单个视图的组。 |
| [setHighlightFilter(boolean value)](#setHighlightFilter-boolean-) | 设置一个值，指示 Microsoft Project 是否突出显示单个视图的筛选器。 |
| [setName(String value)](#setName-java.lang.String-) | 设置 View 对象的名称。 |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | 设置一个值，指示 Microsoft Project 是否在功能区的 View 或 Other Views 下拉列表中显示单个视图的名称。 |
| [setTable(Table value)](#setTable-com.aspose.tasks.Table-) | 设置单个视图的表格。 |
### View() {#View--}
```
public View()
```


初始化一个新的 [View](../../com.aspose.tasks/view) 类实例。

### compareTo(View other) {#compareTo-com.aspose.tasks.View-}
```
public final int compareTo(View other)
```


比较当前实例与同类型的另一个对象，并返回一个整数，指示当前实例在排序顺序中是位于该对象之前、之后，还是与其处于相同位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [View](../../com.aspose.tasks/view) | 要与此实例进行比较的指定 View 对象。 |

**Returns:**
int - 一个 32 位有符号整数，指示被比较对象的相对顺序。返回值具有以下含义：值 含义 小于零 此实例在排序顺序中位于 `other` 之前。 零 此实例在排序顺序中与 `other` 位于相同位置。 大于零 此实例在排序顺序中位于 `other` 之后。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


返回一个值，指示此实例是否等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object | 用于与此实例比较的对象。 |

**Returns:**
boolean - **True** 如果指定的对象是具有与此实例相同 Uid 值的 View；否则，**false**。
### forViewScreen(int viewScreen) {#forViewScreen-int-}
```
public static View forViewScreen(int viewScreen)
```


构造一个新的 [View](../../com.aspose.tasks/view) 类实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| viewScreen | int | 视图可以显示的屏幕类型。 |

**Returns:**
[View](../../com.aspose.tasks/view) - Constructed view.
### getFilter() {#getFilter--}
```
public final Filter getFilter()
```


获取在单个视图中使用的筛选器。

**Returns:**
[Filter](../../com.aspose.tasks/filter) - a filter used in a single view.
### getGroup() {#getGroup--}
```
public final Group getGroup()
```


获取单个视图的组。

**Returns:**
[Group](../../com.aspose.tasks/group) - a group of the single view.
### getHighlightFilter() {#getHighlightFilter--}
```
public final boolean getHighlightFilter()
```


获取一个值，指示 Microsoft Project 是否突出显示单个视图的筛选器。

**Returns:**
boolean - 一个值，指示 Microsoft Project 是否突出显示单个视图的筛选器。
### getName() {#getName--}
```
public final String getName()
```


获取 View 对象的名称。

**Returns:**
java.lang.String - View 对象的名称。
### getPageInfo() {#getPageInfo--}
```
public final PageInfo getPageInfo()
```


获取 `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) 类的实例。表示存在于 mpp 文件格式中的页面设置数据。

**Returns:**
[PageInfo](../../com.aspose.tasks/pageinfo) - an instance of the `PageInfo`([getPageInfo()](../../com.aspose.tasks/view\#getPageInfo--)) class.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


获取 View 对象的父对象。只读 [Project](../../com.aspose.tasks/project)。

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### getScreen() {#getScreen--}
```
public final int getScreen()
```


获取单个视图的屏幕类型。只读 [ViewScreen](../../com.aspose.tasks/viewscreen)。

**Returns:**
int - 单个视图的屏幕类型。
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


获取一个值，指示 Microsoft Project 是否在功能区的 View 或 Other Views 下拉列表中显示单个视图的名称。

**Returns:**
boolean - 一个值，指示 Microsoft Project 是否在功能区的 View 或 Other Views 下拉列表中显示单个视图名称。
### getTable() {#getTable--}
```
public final Table getTable()
```


获取单个视图的表格。

**Returns:**
[Table](../../com.aspose.tasks/table) - a table of the single view.
### getType() {#getType--}
```
public final int getType()
```


获取单个视图中项目的类型，例如任务或资源。只读 [ItemType](../../com.aspose.tasks/itemtype)。

**Returns:**
int - 单个视图中项目的类型，例如任务或资源。
### getUid() {#getUid--}
```
public final int getUid()
```


获取视图的唯一标识符。

**Returns:**
int - 视图的唯一标识符。
### getVisualObjectsPlacements() {#getVisualObjectsPlacements--}
```
public final List<VisualObjectPlacement> getVisualObjectsPlacements()
```


获取表示视图中 [OleObject](../../com.aspose.tasks/oleobject) 的放置和外观的对象集合。

**Returns:**
java.util.List&lt;com.aspose.tasks.VisualObjectPlacement&gt; - 表示视图中 [OleObject](../../com.aspose.tasks/oleobject) 的放置和外观的对象集合。
### hashCode() {#hashCode--}
```
public int hashCode()
```


返回 [Resource](../../com.aspose.tasks/resource) 类实例的哈希码值。

**Returns:**
int - 返回此对象的哈希码值。
### op_Equality(View a, View b) {#op-Equality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Equality(View a, View b)
```


返回一个值，指示此实例是否等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | 第一个视图。 |
| b | [View](../../com.aspose.tasks/view) | 第二个视图。 |

**Returns:**
boolean - 一个值，指示此实例是否等于指定的对象
### op_GreaterThan(View a, View b) {#op-GreaterThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThan(View a, View b)
```


返回一个值，指示此实例是否大于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | 第一个视图。 |
| b | [View](../../com.aspose.tasks/view) | 第二个视图。 |

**Returns:**
boolean - 一个值，指示此实例是否大于指定的对象
### op_GreaterThanOrEqual(View a, View b) {#op-GreaterThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_GreaterThanOrEqual(View a, View b)
```


返回一个值，指示此实例是否大于或等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | 第一个视图。 |
| b | [View](../../com.aspose.tasks/view) | 第二个视图。 |

**Returns:**
boolean - 一个值，指示此实例是否大于或等于指定的对象
### op_Inequality(View a, View b) {#op-Inequality-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_Inequality(View a, View b)
```


返回一个值，指示此实例是否不等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | 第一个视图。 |
| b | [View](../../com.aspose.tasks/view) | 第二个视图。 |

**Returns:**
boolean - 一个值，指示此实例是否不等于指定的对象
### op_LessThan(View a, View b) {#op-LessThan-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThan(View a, View b)
```


返回一个值，指示此实例是否小于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | 第一个筛选器。 |
| b | [View](../../com.aspose.tasks/view) | 第二个筛选器。 |

**Returns:**
boolean - 一个值，指示此实例是否小于指定的对象
### op_LessThanOrEqual(View a, View b) {#op-LessThanOrEqual-com.aspose.tasks.View-com.aspose.tasks.View-}
```
public static boolean op_LessThanOrEqual(View a, View b)
```


返回一个值，指示此实例是否小于或等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | [View](../../com.aspose.tasks/view) | 第一个视图。 |
| b | [View](../../com.aspose.tasks/view) | 第二个视图。 |

**Returns:**
boolean - 一个值，指示此实例是否小于或等于指定的对象
### setFilter(Filter value) {#setFilter-com.aspose.tasks.Filter-}
```
public final void setFilter(Filter value)
```


设置在单个视图中使用的筛选器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Filter](../../com.aspose.tasks/filter) | 在单个视图中使用的筛选器。 |

### setGroup(Group value) {#setGroup-com.aspose.tasks.Group-}
```
public final void setGroup(Group value)
```


设置单个视图的组。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Group](../../com.aspose.tasks/group) | 单个视图的组。 |

### setHighlightFilter(boolean value) {#setHighlightFilter-boolean-}
```
public final void setHighlightFilter(boolean value)
```


设置一个值，指示 Microsoft Project 是否突出显示单个视图的筛选器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示 Microsoft Project 是否突出显示单个视图的筛选器。 |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


设置 View 对象的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String | View 对象的名称。 |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


设置一个值，指示 Microsoft Project 是否在功能区的 View 或 Other Views 下拉列表中显示单个视图的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示 Microsoft Project 是否在功能区的 View 或 Other Views 下拉列表中显示单个视图名称。 |

### setTable(Table value) {#setTable-com.aspose.tasks.Table-}
```
public final void setTable(Table value)
```


设置单个视图的表格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Table](../../com.aspose.tasks/table) | 单个视图的表。 |

