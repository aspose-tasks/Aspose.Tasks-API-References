---
title: "TimephasedDataCollection"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "オブジェクトのコレクションを表します。"
type: docs
weight: 321
url: /ja/java/com.aspose.tasks/timephaseddatacollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class TimephasedDataCollection extends AbstractList<TimephasedData>
```

[TimephasedData](../../com.aspose.tasks/timephaseddata) オブジェクトのコレクションを表します。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [TimephasedDataCollection()](#TimephasedDataCollection--) | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [add(TimephasedData item)](#add-com.aspose.tasks.TimephasedData-) | [TimephasedData](../../com.aspose.tasks/timephaseddata) インスタンスをこのコレクション オブジェクトに追加します。 |
| [addRange(Iterable&lt;TimephasedData&gt; timephasedCollection)](#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--) | このコレクションオブジェクトに、[TimephasedData](../../com.aspose.tasks/timephaseddata) インスタンスのコレクションを追加します。 |
| [clear()](#clear--) | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) からすべての項目を削除します。 |
| [containsItem(TimephasedData item)](#containsItem-com.aspose.tasks.TimephasedData-) | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) が特定の値を含むかどうかを判断します。 |
| [copyToTArray(TimephasedData[] array, int arrayIndex)](#copyToTArray-com.aspose.tasks.TimephasedData---int-) | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) の要素を配列にコピーし、特定の配列インデックスから開始します。 |
| [get(int index)](#get-int-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | System.Collections.Generic.ICollection&lt;T&gt; が読み取り専用かどうかを示す値を取得します。 |
| [iterator()](#iterator--) | このコレクションのイテレータを返します。 |
| [remove(TimephasedData item)](#remove-com.aspose.tasks.TimephasedData-) | このコレクションオブジェクトから [TimephasedData](../../com.aspose.tasks/timephaseddata) インスタンスを削除します。 |
| [selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)](#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-) | `startTime` と `finishTime` の間のすべての時間フェーズを選択します。 |
| [set_Item(int index, TimephasedData value)](#set-Item-int-com.aspose.tasks.TimephasedData-) | 指定されたインデックスの要素を設定します。 |
| [size()](#size--) | この [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) オブジェクトに含まれるオブジェクトの数を取得します。 |
| [toList()](#toList--) | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) オブジェクトを [TimephasedData](../../com.aspose.tasks/timephaseddata) オブジェクトのリストに変換します。 |
### TimephasedDataCollection() {#TimephasedDataCollection--}
```
public TimephasedDataCollection()
```


[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) クラスの新しいインスタンスを初期化します。

### add(TimephasedData item) {#add-com.aspose.tasks.TimephasedData-}
```
public final boolean add(TimephasedData item)
```


[TimephasedData](../../com.aspose.tasks/timephaseddata) インスタンスをこのコレクション オブジェクトに追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | 追加する項目。 |

**Returns:**
boolean - アイテムが追加された場合は true、そうでない場合は false。
### addRange(Iterable&lt;TimephasedData&gt; timephasedCollection) {#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--}
```
public final void addRange(Iterable<TimephasedData> timephasedCollection)
```


このコレクションオブジェクトに、[TimephasedData](../../com.aspose.tasks/timephaseddata) インスタンスのコレクションを追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| timephasedCollection | java.lang.Iterable&lt;com.aspose.tasks.TimephasedData&gt; | 追加する [TimephasedData](../../com.aspose.tasks/timephaseddata) オブジェクトのコレクション。 |

### clear() {#clear--}
```
public final void clear()
```


[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) からすべての項目を削除します。

### containsItem(TimephasedData item) {#containsItem-com.aspose.tasks.TimephasedData-}
```
public final boolean containsItem(TimephasedData item)
```


[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) が特定の値を含むかどうかを判断します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | コレクション内で検索するオブジェクト。 |

**Returns:**
boolean - `item` がコレクション内に見つかった場合は true、そうでない場合は false。
### copyToTArray(TimephasedData[] array, int arrayIndex) {#copyToTArray-com.aspose.tasks.TimephasedData---int-}
```
public final void copyToTArray(TimephasedData[] array, int arrayIndex)
```


[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) の要素を配列にコピーし、特定の配列インデックスから開始します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| array | [TimephasedData\[\]](../../com.aspose.tasks/timephaseddata) | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) からコピーされた要素の宛先となる一次元配列です。配列はゼロベースのインデックスを持つ必要があります。 |
| arrayIndex | int | コピーが開始される `array` のゼロベースインデックス。 |

### get(int index) {#get-int-}
```
public TimephasedData get(int index)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | \{@inheritDoc\} |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


System.Collections.Generic.ICollection&lt;T&gt; が読み取り専用かどうかを示す値を取得します。

**Returns:**
boolean - System.Collections.Generic.ICollection&lt;T&gt; が読み取り専用の場合は true、そうでない場合は false。
### iterator() {#iterator--}
```
public final Iterator<TimephasedData> iterator()
```


このコレクションのイテレータを返します。

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.TimephasedData&gt; - このコレクションのイテレータ。
### remove(TimephasedData item) {#remove-com.aspose.tasks.TimephasedData-}
```
public final boolean remove(TimephasedData item)
```


このコレクションオブジェクトから [TimephasedData](../../com.aspose.tasks/timephaseddata) インスタンスを削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | 削除する項目。 |

**Returns:**
boolean - `item` が [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) から正常に削除された場合は true、そうでない場合は false。このメソッドは `item` が [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) に見つからない場合も false を返します。
### selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime) {#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-}
```
public final List<TimephasedData> selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)
```


`startTime` と `finishTime` の間のすべての時間フェーズを選択します。平均ケースで O(log n) の計算量です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| timephasedDataType | バイト | 選択する時間フェーズのタイプ。 |
| startTime | java.util.Date | 区間の開始。 |
| finishTime | java.util.Date | 区間の終了。 |

**Returns:**
java.util.List&lt;com.aspose.tasks.TimephasedData&gt; - Start プロパティで順序付けされた [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) データの新しいリスト インスタンスを返します。
### set_Item(int index, TimephasedData value) {#set-Item-int-com.aspose.tasks.TimephasedData-}
```
public final void set_Item(int index, TimephasedData value)
```


指定されたインデックスの要素を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 設定する要素のゼロベースインデックス。 |
| value | [TimephasedData](../../com.aspose.tasks/timephaseddata) | 設定する要素。 |

### size() {#size--}
```
public final int size()
```


この [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) オブジェクトに含まれるオブジェクトの数を取得します。

**Returns:**
int - この [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) オブジェクトに含まれるオブジェクトの数。
### toList() {#toList--}
```
public final List<TimephasedData> toList()
```


[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) オブジェクトを [TimephasedData](../../com.aspose.tasks/timephaseddata) オブジェクトのリストに変換します。

**Returns:**
java.util.List&lt;com.aspose.tasks.TimephasedData&gt; - [TimephasedData](../../com.aspose.tasks/timephaseddata) オブジェクトのリスト。
