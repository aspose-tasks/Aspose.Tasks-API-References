---
title: "ResourceCollection"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示对象的集合。"
type: docs
weight: 251
url: /zh/java/com.aspose.tasks/resourcecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceCollection extends AbstractList<Resource>
```

表示一个 [Resource](../../com.aspose.tasks/resource) 对象的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add()](#add--) | 在项目资源集合的最后位置添加新资源。 |
| [add(Resource e)](#add-com.aspose.tasks.Resource-) | \{@inheritDoc\} |
| [add(String resourceName)](#add-java.lang.String-) | 在项目资源集合的最后位置添加新资源。 |
| [add(String resourceName, int beforeResourceId)](#add-java.lang.String-int-) | 在项目资源集合的指定位置添加新资源。 |
| [clear()](#clear--) | 不支持直接清除，此方法仅抛出 UnsupportedOperationException。 |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | 返回具有指定 id 的资源。 |
| [getByUid(int uid)](#getByUid-int-) | 返回具有指定 Uid 的资源。 |
| [getParentProject()](#getParentProject--) | 获取 ResourceCollection 对象的父项目。 |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | \{@inheritDoc\} |
| [iterator()](#iterator--) | 返回此集合的枚举器。 |
| [remove(Object o)](#remove-java.lang.Object-) | 这是 Collection 的 remove 方法的存根实现，仅抛出 UnsupportedOperationException。 |
| [size()](#size--) | 获取 ResourceCollection 中包含的元素数量。 |
| [sort(Comparator&lt;? super Resource&gt; comparer)](#sort-java.util.Comparator---super-com.aspose.tasks.Resource--) | \{@inheritDoc\} |
| [toList()](#toList--) | 将 ResourceCollection 对象转换为 [Resource](../../com.aspose.tasks/resource) 对象的列表。 |
### add() {#add--}
```
public final Resource add()
```


在项目资源集合的最后位置添加新资源。

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(Resource e) {#add-com.aspose.tasks.Resource-}
```
public final boolean add(Resource e)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| e | [Resource](../../com.aspose.tasks/resource) | \{@inheritDoc\} |

**Returns:**
布尔 - \{@inheritDoc\}
### add(String resourceName) {#add-java.lang.String-}
```
public final Resource add(String resourceName)
```


在项目资源集合的最后位置添加新资源。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| resourceName | java.lang.String | 资源的名称。 |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(String resourceName, int beforeResourceId) {#add-java.lang.String-int-}
```
public final Resource add(String resourceName, int beforeResourceId)
```


在项目资源集合的指定位置添加新资源。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| resourceName | java.lang.String | 资源的名称。 |
| beforeResourceId | int | 在项目资源集合中前一个资源的位置。 |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### clear() {#clear--}
```
public final void clear()
```


不支持直接清除，此方法仅抛出 UnsupportedOperationException。

### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
布尔 - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public Resource get(int index)
```


(@inheritDoc\}

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | \{@inheritDoc\} |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Resource getById(int id)
```


返回具有指定 id 的资源。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | id | int | 指定的 ID。 |

--------------------

O(1) 复杂度。 |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified id if present; otherwise, null.
### getByUid(int uid) {#getByUid-int-}
```
public final Resource getByUid(int uid)
```


返回具有指定 Uid 的资源。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | uid | int | 指定的 uid。 |

--------------------

O(1) 复杂度。 |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


获取 ResourceCollection 对象的父项目。

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceCollection object.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```




**Returns:**
布尔 - \{@inheritDoc\}
### iterator() {#iterator--}
```
public final Iterator<Resource> iterator()
```


返回此集合的枚举器。

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Resource&gt; - 此集合的枚举器。
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


这是 Collection 的 remove 方法的存根实现，仅抛出 UnsupportedOperationException。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 要删除的项。 |

**Returns:**
boolean - 如果该项已被移除，则为 `true`；否则为 `false`。
### size() {#size--}
```
public final int size()
```


获取 ResourceCollection 中包含的元素数量。

--------------------

只读 `int`。

**Returns:**
int - ResourceCollection 中包含的元素数量。
### sort(Comparator&lt;? super Resource&gt; comparer) {#sort-java.util.Comparator---super-com.aspose.tasks.Resource--}
```
public final void sort(Comparator<? super Resource> comparer)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| comparer | java.util.Comparator&lt;? super com.aspose.tasks.Resource&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Resource> toList()
```


将 ResourceCollection 对象转换为 [Resource](../../com.aspose.tasks/resource) 对象的列表。

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - [Resource](../../com.aspose.tasks/resource) 对象的列表。
