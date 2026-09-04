---
title: "ResourceAssignmentCollection"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示对象的集合。"
type: docs
weight: 250
url: /zh/java/com.aspose.tasks/resourceassignmentcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceAssignmentCollection extends AbstractList<ResourceAssignment>
```

表示一个包含 [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 对象的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(ResourceAssignment item)](#add-com.aspose.tasks.ResourceAssignment-) | 这是 ICollection 的 Add 方法的存根实现，只会抛出 UnsupportedOperationException。 |
| [add(Task task, Resource resource)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-) | 向 ResourceAssignmentCollection 添加新分配。 |
| [add(Task task, Resource resource, double units)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-) | 向 ResourceAssignmentCollection 添加新分配。 |
| [add(Task task, Resource resource, BigDecimal cost)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-) | 向 ResourceAssignmentCollection 添加新分配。 |
| [clear()](#clear--) | 从集合中移除所有项。 |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByUid(int uid)](#getByUid-int-) | 返回具有指定 uid 的分配。 |
| [getParentProject()](#getParentProject--) | 获取 ResourceAssignmentCollection 对象的父项目。 |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | 获取指示此集合是否只读的值。 |
| [iterator()](#iterator--) | 返回此集合的枚举器。 |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | 从集合中移除指定的分配，如果集合不是只读的，否则抛出 UnsupportedOperationException。 |
| [size()](#size--) | 获取 ResourceAssignmentCollection 中包含的对象数量。 |
| [toList()](#toList--) | 将 ResourceAssignmentCollection 对象转换为 [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 对象的列表。 |
### add(ResourceAssignment item) {#add-com.aspose.tasks.ResourceAssignment-}
```
public final boolean add(ResourceAssignment item)
```


这是 ICollection 的 Add 方法的存根实现，只会抛出 UnsupportedOperationException。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | 要删除的项目。 |

**Returns:**
布尔 - \{@inheritDoc\}
### add(Task task, Resource resource) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-}
```
public final ResourceAssignment add(Task task, Resource resource)
```


向 ResourceAssignmentCollection 添加新分配。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 要分配的任务。 |
| resource | [Resource](../../com.aspose.tasks/resource) | 要分配的资源。 |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, double units) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-}
```
public final ResourceAssignment add(Task task, Resource resource, double units)
```


向 ResourceAssignmentCollection 添加新分配。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 要分配的任务。 |
| resource | [Resource](../../com.aspose.tasks/resource) | 要分配的资源。 |
| 单位 | double | 新分配的单位数量。 |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, BigDecimal cost) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-}
```
public final ResourceAssignment add(Task task, Resource resource, BigDecimal cost)
```


向 ResourceAssignmentCollection 添加新分配。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 要分配的任务。 |
| resource | [Resource](../../com.aspose.tasks/resource) | 要分配的成本资源。 |
| 成本 | java.math.BigDecimal | 新分配的成本。 |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### clear() {#clear--}
```
public void clear()
```


从集合中移除所有项。

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
public ResourceAssignment get(int index)
```


(@inheritDoc\}

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### getByUid(int uid) {#getByUid-int-}
```
public final ResourceAssignment getByUid(int uid)
```


返回具有指定 uid 的分配。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | uid | int | 指定的 uid。 |

--------------------

O(1) 复杂度。 |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - ResourceAssignment with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


获取 ResourceAssignmentCollection 对象的父项目。

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceAssignmentCollection object.
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


获取指示此集合是否只读的值。

**Returns:**
boolean - 指示此集合是否只读的值。
### iterator() {#iterator--}
```
public final Iterator<ResourceAssignment> iterator()
```


返回此集合的枚举器。

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.ResourceAssignment&gt; - 此集合的枚举器。
### remove(int index) {#remove-int-}
```
public ResourceAssignment remove(int index)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


从集合中移除指定的分配，如果集合不是只读的，否则抛出 UnsupportedOperationException。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 要移除的分配。 |

**Returns:**
boolean - 如果指定的项已被移除则为 true，否则为 false。
### size() {#size--}
```
public final int size()
```


获取 ResourceAssignmentCollection 中包含的对象数量。

**Returns:**
int - ResourceAssignmentCollection 中包含的对象数量。
### toList() {#toList--}
```
public final List<ResourceAssignment> toList()
```


将 ResourceAssignmentCollection 对象转换为 [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 对象的列表。

**Returns:**
java.util.List&lt;com.aspose.tasks.ResourceAssignment&gt; - [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 对象的列表。
