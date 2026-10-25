---
title: "ViewCollection"
second_title: "Aspose.Tasks for Java API 参考"
description: "包含一个对象列表。"
type: docs
weight: 343
url: /zh/java/com.aspose.tasks/viewcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class ViewCollection extends AbstractCollection<View>
```

包含一个 [View](../../com.aspose.tasks/view) 对象的列表。扩展 `AbstractCollection` 类。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(View item)](#add-com.aspose.tasks.View-) | 将指定的项添加到此集合中。 |
| [clear()](#clear--) | 从此集合中移除所有项。 |
| [contains(View item)](#contains-com.aspose.tasks.View-) | 如果在此集合中找到指定项，则返回 true；否则返回 false。 |
| [copyTo(View[] array, int arrayIndex)](#copyTo-com.aspose.tasks.View---int-) | 将此集合的元素复制到指定数组中，从指定的数组索引开始。 |
| [getByName(String viewName)](#getByName-java.lang.String-) | 搜索具有该名称的 View，并返回集合中的第一次出现。 |
| [getByViewScreen(int screen)](#getByViewScreen-int-) | 搜索具有指定 Screen 属性的 View，并返回集合中的第一次出现。 |
| [getParentProject()](#getParentProject--) | 获取 View 对象的父对象。 |
| [iterator()](#iterator--) | 返回此集合中包含的元素的迭代器。 |
| [remove(View item)](#remove-com.aspose.tasks.View-) | 从此集合中移除特定对象的第一次出现。 |
| [size()](#size--) | 获取此集合中包含的元素数量。 |
| [toList()](#toList--) | 将视图集合转换为 [View](../../com.aspose.tasks/view) 对象的列表。 |
### add(View item) {#add-com.aspose.tasks.View-}
```
public final boolean add(View item)
```


将指定的项添加到此集合中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | 要添加到此集合的指定项。 |

**Returns:**
boolean - 如果操作成功则为 true。
### clear() {#clear--}
```
public final void clear()
```


从此集合中移除所有项。

### contains(View item) {#contains-com.aspose.tasks.View-}
```
public final boolean contains(View item)
```


如果在此集合中找到指定项，则返回 true；否则返回 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | 要查找的指定项。 |

**Returns:**
布尔 - 如果在此集合中找到指定项，则为 true；否则为 false。
### copyTo(View[] array, int arrayIndex) {#copyTo-com.aspose.tasks.View---int-}
```
public final void copyTo(View[] array, int arrayIndex)
```


将此集合的元素复制到指定数组中，从指定的数组索引开始。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| array | [View\[\]](../../com.aspose.tasks/view) | 要复制元素到的指定一维数组 |
| arrayIndex | int | 指定数组中开始复制的零基索引。 |

### getByName(String viewName) {#getByName-java.lang.String-}
```
public final View getByName(String viewName)
```


搜索具有该名称的 View，并返回集合中的第一次出现。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| viewName | java.lang.String | 要搜索的 View 的名称。 |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection with the specified name, if found; otherwise, null.
### getByViewScreen(int screen) {#getByViewScreen-int-}
```
public final View getByViewScreen(int screen)
```


搜索具有指定 Screen 属性的 View，并返回集合中的第一次出现。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| screen | int | [ViewScreen](../../com.aspose.tasks/viewscreen) 枚举值。 |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection which Screen property matches the specified screen argument, if found; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


获取 View 对象的父对象。只读 [Project](../../com.aspose.tasks/project)。

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### iterator() {#iterator--}
```
public Iterator<View> iterator()
```


返回此集合中包含的元素的迭代器。

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.View&gt; - 集合迭代器。
### remove(View item) {#remove-com.aspose.tasks.View-}
```
public final boolean remove(View item)
```


从此集合中移除特定对象的第一次出现。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | 要移除的指定对象。 |

**Returns:**
boolean - 如果成功从此集合中移除指定对象则为 true；否则为 false。
### size() {#size--}
```
public final int size()
```


获取此集合中包含的元素数量。

**Returns:**
int - 此集合中包含的元素数量。
### toList() {#toList--}
```
public final List<View> toList()
```


将视图集合转换为 [View](../../com.aspose.tasks/view) 对象的列表。

**Returns:**
java.util.List&lt;com.aspose.tasks.View&gt; - [View](../../com.aspose.tasks/view) 对象的通用列表。
