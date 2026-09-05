---
title: "RateCollection"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "オブジェクトを含むコレクションを表します。"
type: docs
weight: 234
url: /ja/java/com.aspose.tasks/ratecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractMap

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RateCollection extends AbstractMap<Integer,RateByDateCollection> implements Iterable<Map.Entry<Integer,RateByDateCollection>>
```

[Rate](../../com.aspose.tasks/rate) オブジェクトを含むコレクションを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [add(Date ratesFrom)](#add-java.util.Date-) | このコレクションに新しい [Rate](../../com.aspose.tasks/rate) インスタンスを追加します。 |
| [add(Date ratesFrom, int type)](#add-java.util.Date-int-) | このコレクションに新しい [Rate](../../com.aspose.tasks/rate) インスタンスを追加します。 |
| [clear()](#clear--) | \{@inheritDoc\} |
| [entrySet()](#entrySet--) | (@inheritDoc\} |
| [get(Object key)](#get-java.lang.Object-) | (@inheritDoc\} |
| [getByRateType(int key)](#getByRateType-int-) | 指定されたインデックスの要素を返します。 |
| [getParentResource()](#getParentResource--) | このコレクションの親 [Resource](../../com.aspose.tasks/resource) オブジェクトを取得します。 |
| [isReadOnly()](#isReadOnly--) | このコレクションが読み取り専用かどうかを示す値を取得します。 |
| [iterator()](#iterator--) | このコレクションの列挙子を返します。 |
| [put(Integer key, RateByDateCollection value)](#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-) | (@inheritDoc\} |
| [remove(Rate item)](#remove-com.aspose.tasks.Rate-) | このコレクションから Rate インスタンスを削除します。 |
| [setByRateType(int key, RateByDateCollection value)](#setByRateType-int-com.aspose.tasks.RateByDateCollection-) | 指定されたインデックスの要素を設定します。 |
| [size()](#size--) | RateCollection に含まれる要素数を取得します。 |
| [toList()](#toList--) | [RateCollection](../../com.aspose.tasks/ratecollection) オブジェクトを [Rate](../../com.aspose.tasks/rate) オブジェクトのリストに変換します。 |
| [toList(int type)](#toList-int-) | [RateCollection](../../com.aspose.tasks/ratecollection) オブジェクトを、指定された [RateType](../../com.aspose.tasks/ratetype) タイプでフィルタリングされた [Rate](../../com.aspose.tasks/rate) オブジェクトのリストに変換します。 |
### add(Date ratesFrom) {#add-java.util.Date-}
```
public final Rate add(Date ratesFrom)
```


このコレクションに新しい [Rate](../../com.aspose.tasks/rate) インスタンスを追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ratesFrom | java.util.Date | 新しいレートが有効になる日付です。 |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### add(Date ratesFrom, int type) {#add-java.util.Date-int-}
```
public final Rate add(Date ratesFrom, int type)
```


このコレクションに新しい [Rate](../../com.aspose.tasks/rate) インスタンスを追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ratesFrom | java.util.Date | 新しいレートが有効になる日付です。 |
| type | int | 追加するレートテーブルです。 |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### clear() {#clear--}
```
public final void clear()
```




### entrySet() {#entrySet--}
```
public Set<Map.Entry<Integer,RateByDateCollection>> entrySet()
```


(@inheritDoc\}

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;java.lang.Integer,com.aspose.tasks.RateByDateCollection&gt;&gt; - \\{@inheritDoc\\}
### get(Object key) {#get-java.lang.Object-}
```
public final RateByDateCollection get(Object key)
```


(@inheritDoc\}

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### getByRateType(int key) {#getByRateType-int-}
```
public final RateByDateCollection getByRateType(int key)
```


指定されたインデックスの要素を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| key | int | 取得する要素のゼロベースインデックスです。 |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - the element at the specified index.
### getParentResource() {#getParentResource--}
```
public final Resource getParentResource()
```


このコレクションの親 [Resource](../../com.aspose.tasks/resource) オブジェクトを取得します。

**Returns:**
[Resource](../../com.aspose.tasks/resource) - the parent [Resource](../../com.aspose.tasks/resource) object for this collection.
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


このコレクションが読み取り専用かどうかを示す値を取得します。

**Returns:**
boolean - このコレクションが読み取り専用かどうかを示す値です。
### iterator() {#iterator--}
```
public final Iterator iterator()
```


このコレクションの列挙子を返します。

**Returns:**
java.util.Iterator - このコレクションの列挙子です。
### put(Integer key, RateByDateCollection value) {#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-}
```
public final RateByDateCollection put(Integer key, RateByDateCollection value)
```


(@inheritDoc\}

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| key | java.lang.Integer | \{@inheritDoc\} |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### remove(Rate item) {#remove-com.aspose.tasks.Rate-}
```
public final boolean remove(Rate item)
```


このコレクションから Rate インスタンスを削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| item | [Rate](../../com.aspose.tasks/rate) | 削除する項目。 |

**Returns:**
boolean - 指定された Rate が正常に削除された場合は true、そうでない場合は false。
### setByRateType(int key, RateByDateCollection value) {#setByRateType-int-com.aspose.tasks.RateByDateCollection-}
```
public final void setByRateType(int key, RateByDateCollection value)
```


指定されたインデックスの要素を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| key | int | 設定する要素のゼロベースインデックス。 |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | 指定されたインデックスに設定する要素。 |

### size() {#size--}
```
public final int size()
```


RateCollection に含まれる要素数を取得します。

**Returns:**
int - RateCollection に含まれる要素数。
### toList() {#toList--}
```
public final List<Rate> toList()
```


[RateCollection](../../com.aspose.tasks/ratecollection) オブジェクトを [Rate](../../com.aspose.tasks/rate) オブジェクトのリストに変換します。

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - [Rate](../../com.aspose.tasks/rate) オブジェクトのリスト。
### toList(int type) {#toList-int-}
```
public final List<Rate> toList(int type)
```


[RateCollection](../../com.aspose.tasks/ratecollection) オブジェクトを、指定された [RateType](../../com.aspose.tasks/ratetype) タイプでフィルタリングされた [Rate](../../com.aspose.tasks/rate) オブジェクトのリストに変換します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| type | int | フィルタ対象の型。 |

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - [Rate](../../com.aspose.tasks/rate) オブジェクトのリスト。
