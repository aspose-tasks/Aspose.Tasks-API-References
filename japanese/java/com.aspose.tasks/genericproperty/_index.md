---
title: "GenericProperty"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "コンテナ プロパティを表します。"
type: docs
weight: 113
url: /ja/java/com.aspose.tasks/genericproperty/
---

**Inheritance:**
java.lang.Object
```
public class GenericProperty<TKey>
```

コンテナ プロパティを表します。

TKey : プロパティ値の型です。
## コンストラクター

| コンストラクター | 説明 |
| --- | --- |
| [GenericProperty()](#GenericProperty--) | GenericProperty&lt;T&gt; クラスの新しいインスタンスを初期化します。 |
| [GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name)](#GenericProperty-java.lang.Class-TKey--java.lang.String-) | GenericProperty&lt;TKey&gt; 構造体の新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [&lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2)](#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--) | 指定された `obj1` インスタンスが指定された `obj2` インスタンスと等しいかどうかを示す値を返します。 |
| [Clone()](#Clone--) | このインスタンスのディープコピーを作成して返します。 |
| [CloneTo(GenericProperty&lt;TKey&gt; that)](#CloneTo-com.aspose.tasks.GenericProperty-TKey--) | インスタンスのディープコピーを別のインスタンスに作成します。 |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getName()](#getName--) | プロパティの名前を取得します。 |
| [getValue()](#getValue--) | プロパティの値を取得します。 |
### GenericProperty() {#GenericProperty--}
```
public GenericProperty()
```


GenericProperty&lt;T&gt; クラスの新しいインスタンスを初期化します。

### GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name) {#GenericProperty-java.lang.Class-TKey--java.lang.String-}
```
public GenericProperty(Class<TKey> typeOfTKey, String name)
```


GenericProperty&lt;TKey&gt; 構造体の新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| typeOfTKey | java.lang.Class&lt;TKey&gt; |  |
| name | java.lang.String | プロパティの名前。 |

### &lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2) {#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--}
```
public static boolean <TKey>equals(GenericProperty<TKey> obj1, GenericProperty<TKey> obj2)
```


指定された `obj1` インスタンスが指定された `obj2` インスタンスと等しいかどうかを示す値を返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| obj1 | [GenericProperty](../../com.aspose.tasks/genericproperty) | 比較する最初のオブジェクト。 |
| obj2 | [GenericProperty](../../com.aspose.tasks/genericproperty) | 比較する2番目のオブジェクト。 |

**Returns:**
boolean - 指定された `obj1` インスタンスが指定された `obj2` インスタンスと等しい場合は true を返し、そうでない場合は false を返します。
### Clone() {#Clone--}
```
public GenericProperty<TKey> Clone()
```


このインスタンスのディープコピーを作成して返します。

**Returns:**
[GenericProperty](../../com.aspose.tasks/genericproperty) - a deep copy of this object.
### CloneTo(GenericProperty&lt;TKey&gt; that) {#CloneTo-com.aspose.tasks.GenericProperty-TKey--}
```
public void CloneTo(GenericProperty<TKey> that)
```


インスタンスのディープコピーを別のインスタンスに作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| that | [GenericProperty](../../com.aspose.tasks/genericproperty) | 別のインスタンス。 |

### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
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
### getName() {#getName--}
```
public final String getName()
```


プロパティの名前を取得します。

**Returns:**
java.lang.String - プロパティの名前。
### getValue() {#getValue--}
```
public final Object getValue()
```


プロパティの値を取得します。

**Returns:**
java.lang.Object - プロパティの値。
