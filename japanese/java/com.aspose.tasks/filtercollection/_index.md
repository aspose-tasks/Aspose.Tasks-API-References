---
title: "FilterCollection"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "オブジェクトのリストを含みます。"
type: docs
weight: 92
url: /ja/java/com.aspose.tasks/filtercollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class FilterCollection extends AbstractCollection<Filter>
```

[Filter](../../com.aspose.tasks/filter) オブジェクトのリストを含みます。ICollection&lt;Filter&gt; インターフェイスを実装します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [add(Filter item)](#add-com.aspose.tasks.Filter-) |  |
| [clear()](#clear--) | このコレクションからすべての要素を削除します（オプション操作）。 |
| [contains(Filter item)](#contains-com.aspose.tasks.Filter-) | このコレクションが指定された項目を含む場合、true を返します。 |
| [copyTo(Filter[] array, int arrayIndex)](#copyTo-com.aspose.tasks.Filter---int-) | 指定された配列からこのコレクションへ、指定されたインデックスから要素をコピーします。 |
| [iterator()](#iterator--) | このコレクションに含まれる要素のイテレータを返します。 |
| [remove(Filter item)](#remove-com.aspose.tasks.Filter-) | このコレクションから指定された項目を削除します。 |
| [size()](#size--) | このコレクションに含まれる要素数を取得します。 |
| [toList()](#toList--) | `Filter` オブジェクトのリストにフィルタコレクションを変換します。 |
### add(Filter item) {#add-com.aspose.tasks.Filter-}
```
public boolean add(Filter item)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) |  |

**Returns:**
boolean
### clear() {#clear--}
```
public void clear()
```


このコレクションからすべての要素を削除します（オプション操作）。

### contains(Filter item) {#contains-com.aspose.tasks.Filter-}
```
public final boolean contains(Filter item)
```


このコレクションが指定された項目を含む場合、true を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | 指定された項目。 |

**Returns:**
boolean - コレクションが指定された項目を含む場合は true。
### copyTo(Filter[] array, int arrayIndex) {#copyTo-com.aspose.tasks.Filter---int-}
```
public final void copyTo(Filter[] array, int arrayIndex)
```


指定された配列からこのコレクションへ、指定されたインデックスから要素をコピーします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| array | [Filter\[\]](../../com.aspose.tasks/filter) | 要素をコピーする先の指定された一次元配列 |
| arrayIndex | int | コピーが開始される指定された配列のゼロベースインデックス。 |

### iterator() {#iterator--}
```
public Iterator<Filter> iterator()
```


このコレクションに含まれる要素のイテレータを返します。

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Filter&gt; - コレクションイテレータ。
### remove(Filter item) {#remove-com.aspose.tasks.Filter-}
```
public final boolean remove(Filter item)
```


このコレクションから指定された項目を削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | 指定された項目。 |

**Returns:**
boolean - 操作が成功した場合は true。
### size() {#size--}
```
public final int size()
```


このコレクションに含まれる要素数を取得します。

**Returns:**
int - このコレクションに含まれる要素数。
### toList() {#toList--}
```
public List<Filter> toList()
```


`Filter` オブジェクトのリストにフィルタコレクションを変換します。

**Returns:**
java.util.List&lt;com.aspose.tasks.Filter&gt; - `Filter` オブジェクトの汎用リスト。
