---
title: "PropertyKeyedCollection"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "プロパティコレクションの基底クラスです。"
type: docs
weight: 231
url: /ja/java/com.aspose.tasks/propertykeyedcollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection

**All Implemented Interfaces:**
java.util.Collection
```
public abstract class PropertyKeyedCollection<T> extends PropertyCollection<T> implements Collection<T>
```

プロパティコレクションの基底クラスです。

T : プロパティの型。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [&lt;T1&gt;toArray(T1[] a)](#-T1-toArray-T1---) | \{@inheritDoc\} |
| [add(T item)](#add-T-) | 新しいカスタムプロパティを作成します。 |
| [addAll(Collection&lt;? extends T&gt; c)](#addAll-java.util.Collection---extends-T--) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object item)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [contains(String name)](#contains-java.lang.String-) | Aspose.Tasks.Properties.PropertyCollection&lt;T&gt; が指定された名前のプロパティを含むかどうかを判断します。 |
| [containsAll(Collection&lt;?&gt; c)](#containsAll-java.util.Collection----) | \{@inheritDoc\} |
| [getNames()](#getNames--) | すべてのプロパティ名のコレクションを取得します。 |
| [get_Item(String name)](#get-Item-java.lang.String-) | 指定されたキーに関連付けられた Property を取得します。 |
| [isEmpty()](#isEmpty--) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | このコレクションが読み取り専用かどうかを示す値を取得します。そうでなければ false です。 |
| [remove(Object item)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [removeAll(Collection&lt;?&gt; c)](#removeAll-java.util.Collection----) | \{@inheritDoc\} |
| [retainAll(Collection&lt;?&gt; c)](#retainAll-java.util.Collection----) | \{@inheritDoc\} |
| [size()](#size--) | コレクション内のプロパティ数を取得します。 |
| [toArray()](#toArray--) | \{@inheritDoc\} |
### &lt;T1&gt;toArray(T1[] a) {#-T1-toArray-T1---}
```
public T1[] <T1>toArray(T1[] a)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| a | T1[] | \{@inheritDoc\} |

**Returns:**
T1[] - \{@inheritDoc\}
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


新しいカスタムプロパティを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| アイテム | T | 追加するプロパティ。 |

**Returns:**
boolean
### addAll(Collection&lt;? extends T&gt; c) {#addAll-java.util.Collection---extends-T--}
```
public boolean addAll(Collection<? extends T> c)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| c | java.util.Collection&lt;? extends T&gt; | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public void clear()
```




### contains(Object item) {#contains-java.lang.Object-}
```
public final boolean contains(Object item)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| アイテム | java.lang.Object |  |

**Returns:**
boolean
### contains(String name) {#contains-java.lang.String-}
```
public final boolean contains(String name)
```


Aspose.Tasks.Properties.PropertyCollection&lt;T&gt; が指定された名前のプロパティを含むかどうかを判断します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | java.lang.String | プロパティの名前 |

**Returns:**
boolean - 指定された名前のプロパティが Aspose.Tasks.Properties.PropertyCollection<T> に含まれている場合は true、そうでない場合は false。
### containsAll(Collection&lt;?&gt; c) {#containsAll-java.util.Collection----}
```
public boolean containsAll(Collection<?> c)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| c | java.util.Collection<?> | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### getNames() {#getNames--}
```
public final Collection<String> getNames()
```


すべてのプロパティ名のコレクションを取得します。

**Returns:**
java.util.Collection<java.lang.String> - すべてのプロパティ名のコレクション。
### get_Item(String name) {#get-Item-java.lang.String-}
```
public final T get_Item(String name)
```


指定されたキーに関連付けられた Property を取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | java.lang.String | 取得するプロパティの名前。 |

**Returns:**
T - 指定された名前に関連付けられたプロパティ。
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```




**Returns:**
boolean - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


このコレクションが読み取り専用かどうかを示す値を取得します。そうでなければ false です。

**Returns:**
boolean - このコレクションが読み取り専用かどうかを示す値。そうでなければ false。
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| アイテム | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### removeAll(Collection&lt;?&gt; c) {#removeAll-java.util.Collection----}
```
public boolean removeAll(Collection<?> c)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| c | java.util.Collection<?> | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### retainAll(Collection&lt;?&gt; c) {#retainAll-java.util.Collection----}
```
public boolean retainAll(Collection<?> c)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| c | java.util.Collection<?> | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


コレクション内のプロパティ数を取得します。

**Returns:**
int - コレクション内のプロパティ数。
### toArray() {#toArray--}
```
public Object[] toArray()
```




**Returns:**
java.lang.Object[] - {@inheritDoc}
