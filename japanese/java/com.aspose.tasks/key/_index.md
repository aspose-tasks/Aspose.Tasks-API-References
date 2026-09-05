---
title: "キー"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "指定されたタイプのクラスのプロパティキーを表します。"
type: docs
weight: 139
url: /ja/java/com.aspose.tasks/key/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct
```
public class Key<T,K> extends Struct<Key<T,K>>
```

指定された型のクラスのプロパティキーを表します。このクラスのインスタンスは、コンテナのプロパティを取得または設定する際に使用されます。

T : プロパティ値の型です。
K : プロパティキーの型です。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [Clone()](#Clone--) | インスタンスのディープコピーを返します。 |
| [CloneTo(Key&lt;T,K&gt; that)](#CloneTo-com.aspose.tasks.Key-T-K--) | インスタンスのディープコピーを別のインスタンスに作成します。 |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Key obj1, Key obj2)](#equals-com.aspose.tasks.Key-com.aspose.tasks.Key-) | 指定された `obj1` インスタンスが指定された `obj2` インスタンスと等しいかどうかを示す値を返します。 |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getKeyType()](#getKeyType--) | プロパティのキーを取得します。 |
| [hashCode()](#hashCode--) | Key クラスのインスタンスのハッシュコードを返します。 |
### Clone() {#Clone--}
```
public Key<T,K> Clone()
```


インスタンスのディープコピーを返します。

**Returns:**
[Key](../../com.aspose.tasks/key) - deep copy of the instance.
### CloneTo(Key&lt;T,K&gt; that) {#CloneTo-com.aspose.tasks.Key-T-K--}
```
public void CloneTo(Key<T,K> that)
```


インスタンスのディープコピーを別のインスタンスに作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| that | [Key](../../com.aspose.tasks/key) | 別のインスタンス。 |

### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### equals(Key obj1, Key obj2) {#equals-com.aspose.tasks.Key-com.aspose.tasks.Key-}
```
public static boolean equals(Key obj1, Key obj2)
```


指定された `obj1` インスタンスが指定された `obj2` インスタンスと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| obj1 | com.aspose.tasks.Key | 比較する最初のオブジェクト。 |
| obj2 | com.aspose.tasks.Key | 比較する2番目のオブジェクト。 |

**Returns:**
boolean - 指定された `obj1` インスタンスが指定された `obj2` インスタンスと等しい場合は true を返し、そうでない場合は false を返します。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| obj | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### getKeyType() {#getKeyType--}
```
public final K getKeyType()
```


プロパティのキーを取得します。

**Returns:**
K - プロパティのキーです。
### hashCode() {#hashCode--}
```
public int hashCode()
```


Key クラスのインスタンスのハッシュコードを返します。

**Returns:**
int - このオブジェクトのハッシュコードを返します。
