---
title: "ResourceAssignmentCollection"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "オブジェクトのコレクションを表します。"
type: docs
weight: 250
url: /ja/java/com.aspose.tasks/resourceassignmentcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceAssignmentCollection extends AbstractList<ResourceAssignment>
```

[ResourceAssignment](../../com.aspose.tasks/resourceassignment) オブジェクトのコレクションを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [add(ResourceAssignment item)](#add-com.aspose.tasks.ResourceAssignment-) | これは ICollection の Add メソッドのスタブ実装で、UnsupportedOperationException をスローするだけです。 |
| [add(Task task, Resource resource)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-) | ResourceAssignmentCollection に新しい割り当てを追加します。 |
| [add(Task task, Resource resource, double units)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-) | ResourceAssignmentCollection に新しい割り当てを追加します。 |
| [add(Task task, Resource resource, BigDecimal cost)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-) | ResourceAssignmentCollection に新しい割り当てを追加します。 |
| [clear()](#clear--) | コレクションからすべての項目を削除します。 |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByUid(int uid)](#getByUid-int-) | 指定された uid を持つ割り当てを返します。 |
| [getParentProject()](#getParentProject--) | ResourceAssignmentCollection オブジェクトの親プロジェクトを取得します。 |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | このコレクションが読み取り専用かどうかを示す値を取得します。 |
| [iterator()](#iterator--) | このコレクションの列挙子を返します。 |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | コレクションから指定された割り当てを削除します（読み取り専用でない場合）。読み取り専用の場合は UnsupportedOperationException をスローします。 |
| [size()](#size--) | ResourceAssignmentCollection に含まれるオブジェクトの数を取得します。 |
| [toList()](#toList--) | ResourceAssignmentCollection オブジェクトを [ResourceAssignment](../../com.aspose.tasks/resourceassignment) オブジェクトのリストに変換します。 |
### add(ResourceAssignment item) {#add-com.aspose.tasks.ResourceAssignment-}
```
public final boolean add(ResourceAssignment item)
```


これは ICollection の Add メソッドのスタブ実装で、UnsupportedOperationException をスローするだけです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| item | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | 削除する項目。 |

**Returns:**
boolean - \{@inheritDoc\}
### add(Task task, Resource resource) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-}
```
public final ResourceAssignment add(Task task, Resource resource)
```


ResourceAssignmentCollection に新しい割り当てを追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 割り当てられるタスク。 |
| resource | [Resource](../../com.aspose.tasks/resource) | 割り当てられるリソース。 |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, double units) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-}
```
public final ResourceAssignment add(Task task, Resource resource, double units)
```


ResourceAssignmentCollection に新しい割り当てを追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 割り当てられるタスク。 |
| resource | [Resource](../../com.aspose.tasks/resource) | 割り当てられるリソース。 |
| 単位 | double | 新しい割り当ての単位数。 |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, BigDecimal cost) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-}
```
public final ResourceAssignment add(Task task, Resource resource, BigDecimal cost)
```


ResourceAssignmentCollection に新しい割り当てを追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 割り当てられるタスク。 |
| resource | [Resource](../../com.aspose.tasks/resource) | 割り当てられるコストリソース。 |
| コスト | java.math.BigDecimal | 新しい割り当てのコスト。 |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### clear() {#clear--}
```
public void clear()
```


コレクションからすべての項目を削除します。

### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public ResourceAssignment get(int index)
```


(@inheritDoc\}

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### getByUid(int uid) {#getByUid-int-}
```
public final ResourceAssignment getByUid(int uid)
```


指定された uid を持つ割り当てを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | uid | int | 指定された uid。 |

--------------------

O(1) の計算量。 |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - ResourceAssignment with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


ResourceAssignmentCollection オブジェクトの親プロジェクトを取得します。

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceAssignmentCollection object.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


このコレクションが読み取り専用かどうかを示す値を取得します。

**Returns:**
boolean - このコレクションが読み取り専用かどうかを示す値です。
### iterator() {#iterator--}
```
public final Iterator<ResourceAssignment> iterator()
```


このコレクションの列挙子を返します。

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.ResourceAssignment&gt; - このコレクションの列挙子です。
### remove(int index) {#remove-int-}
```
public ResourceAssignment remove(int index)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


コレクションから指定された割り当てを削除します（読み取り専用でない場合）。読み取り専用の場合は UnsupportedOperationException をスローします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| o | java.lang.Object | 削除する割り当て。 |

**Returns:**
boolean - 指定された項目が削除された場合は true、そうでない場合は false。
### size() {#size--}
```
public final int size()
```


ResourceAssignmentCollection に含まれるオブジェクトの数を取得します。

**Returns:**
int - ResourceAssignmentCollection に含まれるオブジェクトの数。
### toList() {#toList--}
```
public final List<ResourceAssignment> toList()
```


ResourceAssignmentCollection オブジェクトを [ResourceAssignment](../../com.aspose.tasks/resourceassignment) オブジェクトのリストに変換します。

**Returns:**
java.util.List&lt;com.aspose.tasks.ResourceAssignment&gt; - [ResourceAssignment](../../com.aspose.tasks/resourceassignment) オブジェクトのリストです。
