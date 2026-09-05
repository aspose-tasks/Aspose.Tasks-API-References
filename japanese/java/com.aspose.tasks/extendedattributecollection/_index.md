---
title: "ExtendedAttributeCollection"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "オブジェクトのコレクションを表します。"
type: docs
weight: 82
url: /ja/java/com.aspose.tasks/extendedattributecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ExtendedAttributeCollection extends AbstractList<ExtendedAttribute>
```

[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) オブジェクトのコレクションを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [add(ExtendedAttribute item)](#add-com.aspose.tasks.ExtendedAttribute-) | 指定された項目をこのコレクションに追加します。 |
| [clear()](#clear--) | このコレクションからすべての項目を削除します。 |
| [contains(ExtendedAttribute item)](#contains-com.aspose.tasks.ExtendedAttribute-) | 指定された項目がこのコレクションに見つかった場合は true を返し、そうでない場合は false を返します。 |
| [copyTo(ExtendedAttribute[] array, int arrayIndex)](#copyTo-com.aspose.tasks.ExtendedAttribute---int-) | このコレクションの要素を、指定された配列インデックスから開始して、指定された配列にコピーします。 |
| [get(int index)](#get-int-) | 指定されたインデックスの要素を取得します。 |
| [indexOf(ExtendedAttribute item)](#indexOf-com.aspose.tasks.ExtendedAttribute-) | このコレクション内で指定された項目のインデックスを決定します。 |
| [insert(int index, ExtendedAttribute item)](#insert-int-com.aspose.tasks.ExtendedAttribute-) | 指定されたインデックスに指定された項目を挿入します。 |
| [iterator()](#iterator--) | このコレクションの要素に対するイテレータを返します。 |
| [remove(int index)](#remove-int-) | 指定されたインデックスの項目を削除します。 |
| [remove(Object item)](#remove-java.lang.Object-) | コレクションから要素を削除します。 |
| [set(int index, ExtendedAttribute value)](#set-int-com.aspose.tasks.ExtendedAttribute-) | このリストの指定された位置にある要素を、指定された要素に置き換えます。 |
| [size()](#size--) | このコレクションに含まれる要素数を取得します。 |
### add(ExtendedAttribute item) {#add-com.aspose.tasks.ExtendedAttribute-}
```
public final boolean add(ExtendedAttribute item)
```


指定された項目をこのコレクションに追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| item | [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) | このコレクションに追加する指定された項目。 |

**Returns:**
ブール値 - 指定された項目が正常に追加された場合は true、そうでない場合は false。
### clear() {#clear--}
```
public final void clear()
```


このコレクションからすべての項目を削除します。

### contains(ExtendedAttribute item) {#contains-com.aspose.tasks.ExtendedAttribute-}
```
public final boolean contains(ExtendedAttribute item)
```


指定された項目がこのコレクションに見つかった場合は true を返し、そうでない場合は false を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| item | [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) | 検索する指定された項目。 |

**Returns:**
boolean - 指定された項目がこのコレクションに見つかった場合は true、そうでない場合は false。
### copyTo(ExtendedAttribute[] array, int arrayIndex) {#copyTo-com.aspose.tasks.ExtendedAttribute---int-}
```
public final void copyTo(ExtendedAttribute[] array, int arrayIndex)
```


このコレクションの要素を、指定された配列インデックスから開始して、指定された配列にコピーします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| array | [ExtendedAttribute\[\]](../../com.aspose.tasks/extendedattribute) | 要素をコピーする先の指定された一次元配列 |
| arrayIndex | int | コピーが開始される指定された配列のゼロベースインデックス。 |

### get(int index) {#get-int-}
```
public final ExtendedAttribute get(int index)
```


指定されたインデックスの要素を取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 取得または設定する要素のゼロベースインデックスです。 |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - the element at the specified index.
### indexOf(ExtendedAttribute item) {#indexOf-com.aspose.tasks.ExtendedAttribute-}
```
public final int indexOf(ExtendedAttribute item)
```


このコレクション内で指定された項目のインデックスを決定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| item | [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) | このコレクション内で検索する指定された項目です。 |

**Returns:**
int - 見つかった場合の指定項目のインデックス。見つからない場合は -1。
### insert(int index, ExtendedAttribute item) {#insert-int-com.aspose.tasks.ExtendedAttribute-}
```
public final void insert(int index, ExtendedAttribute item)
```


指定されたインデックスに指定された項目を挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 項目を挿入すべき指定されたゼロベースインデックスです。 |
| item | [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) | このコレクションに挿入する指定された項目です。 |

### iterator() {#iterator--}
```
public Iterator<ExtendedAttribute> iterator()
```


このコレクションの要素に対するイテレータを返します。

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.ExtendedAttribute&gt; - このコレクションの要素を反復処理するイテレータです。
### remove(int index) {#remove-int-}
```
public final ExtendedAttribute remove(int index)
```


指定されたインデックスの項目を削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 項目を削除する指定されたゼロベースインデックスです。 |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - the element that was removed from the collection.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


コレクションから要素を削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| アイテム | java.lang.Object | 削除する要素です。 |

**Returns:**
boolean - 要素がコレクションから削除された場合は true、そうでない場合は false。
### set(int index, ExtendedAttribute value) {#set-int-com.aspose.tasks.ExtendedAttribute-}
```
public final ExtendedAttribute set(int index, ExtendedAttribute value)
```


このリストの指定された位置にある要素を、指定された要素に置き換えます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 要素を置き換える指定された位置です。 |
| value | [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) | 指定された位置の要素を置き換える指定された要素です。 |

**Returns:**
[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) - the element replaced by the specified element at the specified position.
### size() {#size--}
```
public final int size()
```


このコレクションに含まれる要素数を取得します。

**Returns:**
int - このコレクションに含まれる要素数。
