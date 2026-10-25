---
title: "ReadOnlyCollectionBase"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "オブジェクトの読み取り専用コレクションを表します。"
type: docs
weight: 238
url: /ja/java/com.aspose.tasks/readonlycollectionbase/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class ReadOnlyCollectionBase<T> extends AbstractList<T>
```

オブジェクトの読み取り専用コレクションを表します。

T : コレクション項目の型。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [add(T item)](#add-T-) | これは ICollection の Add メソッドのスタブ実装で、UnsupportedOperationException をスローするだけです。 |
| [add(int index, T element)](#add-int-T-) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | 指定されたインデックスの要素を返します。 |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | コレクションが読み取り専用かどうかを判定します。 |
| [iterator()](#iterator--) | このコレクションの列挙子を返します。 |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [set(int index, T value)](#set-int-T-) | 指定されたインデックスの要素を返します。 |
| [size()](#size--) | オブジェクトに含まれるオブジェクト数を取得します。 |
| [toList()](#toList--) | コレクションをオブジェクトのリストに変換します。 |
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


これは ICollection の Add メソッドのスタブ実装で、UnsupportedOperationException をスローするだけです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| アイテム | T | 追加する項目。 |

**Returns:**
boolean
### add(int index, T element) {#add-int-T-}
```
public final void add(int index, T element)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | \{@inheritDoc\} |
| 要素 | T | \{@inheritDoc\} |

### clear() {#clear--}
```
public final void clear()
```




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
public final T get(int index)
```


指定されたインデックスの要素を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 取得する要素のゼロベースインデックスです。 |

**Returns:**
T - 指定されたインデックスの要素。
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


コレクションが読み取り専用かどうかを判定します。

**Returns:**
boolean - コレクションが読み取り専用の場合は true、そうでない場合は false。
### iterator() {#iterator--}
```
public final Iterator<T> iterator()
```


このコレクションの列挙子を返します。

**Returns:**
java.util.Iterator<T> - このコレクションの列挙子。
### remove(int index) {#remove-int-}
```
public final T remove(int index)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | \{@inheritDoc\} |

**Returns:**
T - {@inheritDoc}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### set(int index, T value) {#set-int-T-}
```
public final T set(int index, T value)
```


指定されたインデックスの要素を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | 取得する要素のゼロベースインデックスです。 |
| 値 | T |  |

**Returns:**
T - 指定されたインデックスの要素。
### size() {#size--}
```
public final int size()
```


オブジェクトに含まれるオブジェクト数を取得します。

**Returns:**
int - オブジェクトに含まれるオブジェクト数。
### toList() {#toList--}
```
public final List<T> toList()
```


コレクションをオブジェクトのリストに変換します。

**Returns:**
java.util.List<T> - オブジェクトの汎用リスト。
