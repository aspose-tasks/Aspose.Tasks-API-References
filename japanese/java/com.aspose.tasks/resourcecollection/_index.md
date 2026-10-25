---
title: "ResourceCollection"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "オブジェクトのコレクションを表します。"
type: docs
weight: 251
url: /ja/java/com.aspose.tasks/resourcecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceCollection extends AbstractList<Resource>
```

[Resource](../../com.aspose.tasks/resource) オブジェクトのコレクションを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [add()](#add--) | プロジェクトのリソースコレクションの最後の位置に新しいリソースを追加します。 |
| [add(Resource e)](#add-com.aspose.tasks.Resource-) | \{@inheritDoc\} |
| [add(String resourceName)](#add-java.lang.String-) | プロジェクトのリソースコレクションの最後の位置に新しいリソースを追加します。 |
| [add(String resourceName, int beforeResourceId)](#add-java.lang.String-int-) | プロジェクトのリソースコレクションの指定された位置に新しいリソースを追加します。 |
| [clear()](#clear--) | 直接クリアはサポートされておらず、このメソッドは UnsupportedOperationException をスローするだけです。 |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | 指定された id のリソースを返します。 |
| [getByUid(int uid)](#getByUid-int-) | 指定された Uid のリソースを返します。 |
| [getParentProject()](#getParentProject--) | ResourceCollection オブジェクトの親プロジェクトを取得します。 |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | \{@inheritDoc\} |
| [iterator()](#iterator--) | このコレクションの列挙子を返します。 |
| [remove(Object o)](#remove-java.lang.Object-) | これは Collection の remove メソッドのスタブ実装で、UnsupportedOperationException をスローするだけです。 |
| [size()](#size--) | ResourceCollection に含まれる要素数を取得します。 |
| [sort(Comparator&lt;? super Resource&gt; comparer)](#sort-java.util.Comparator---super-com.aspose.tasks.Resource--) | \{@inheritDoc\} |
| [toList()](#toList--) | ResourceCollection オブジェクトを [Resource](../../com.aspose.tasks/resource) オブジェクトのリストに変換します。 |
### add() {#add--}
```
public final Resource add()
```


プロジェクトのリソースコレクションの最後の位置に新しいリソースを追加します。

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(Resource e) {#add-com.aspose.tasks.Resource-}
```
public final boolean add(Resource e)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| e | [Resource](../../com.aspose.tasks/resource) | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### add(String resourceName) {#add-java.lang.String-}
```
public final Resource add(String resourceName)
```


プロジェクトのリソースコレクションの最後の位置に新しいリソースを追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| resourceName | java.lang.String | リソースの名前。 |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(String resourceName, int beforeResourceId) {#add-java.lang.String-int-}
```
public final Resource add(String resourceName, int beforeResourceId)
```


プロジェクトのリソースコレクションの指定された位置に新しいリソースを追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| resourceName | java.lang.String | リソースの名前。 |
| beforeResourceId | int | プロジェクトのリソースコレクション内で前のリソースの位置。 |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### clear() {#clear--}
```
public final void clear()
```


直接クリアはサポートされておらず、このメソッドは UnsupportedOperationException をスローするだけです。

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
public Resource get(int index)
```


(@inheritDoc\}

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | \{@inheritDoc\} |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Resource getById(int id)
```


指定された id のリソースを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | id | int | 指定された ID。 |

--------------------

O(1) の計算量。 |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified id if present; otherwise, null.
### getByUid(int uid) {#getByUid-int-}
```
public final Resource getByUid(int uid)
```


指定された Uid のリソースを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | uid | int | 指定された uid。 |

--------------------

O(1) の計算量。 |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


ResourceCollection オブジェクトの親プロジェクトを取得します。

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceCollection object.
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




**Returns:**
boolean - \{@inheritDoc\}
### iterator() {#iterator--}
```
public final Iterator<Resource> iterator()
```


このコレクションの列挙子を返します。

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Resource&gt; - このコレクションの列挙子。
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


これは Collection の remove メソッドのスタブ実装で、UnsupportedOperationException をスローするだけです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| o | java.lang.Object | 削除する項目。 |

**Returns:**
boolean - アイテムが削除された場合は `true`、それ以外は `false`。
### size() {#size--}
```
public final int size()
```


ResourceCollection に含まれる要素数を取得します。

--------------------

読み取り専用 `int`。

**Returns:**
int - ResourceCollection に含まれる要素数。
### sort(Comparator&lt;? super Resource&gt; comparer) {#sort-java.util.Comparator---super-com.aspose.tasks.Resource--}
```
public final void sort(Comparator<? super Resource> comparer)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 比較子 | java.util.Comparator&lt;? super com.aspose.tasks.Resource&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Resource> toList()
```


ResourceCollection オブジェクトを [Resource](../../com.aspose.tasks/resource) オブジェクトのリストに変換します。

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - [Resource](../../com.aspose.tasks/resource) オブジェクトのリスト。
