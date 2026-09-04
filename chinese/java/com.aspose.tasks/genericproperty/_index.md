---
title: "GenericProperty"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示容器属性。"
type: docs
weight: 113
url: /zh/java/com.aspose.tasks/genericproperty/
---

**Inheritance:**
java.lang.Object
```
public class GenericProperty<TKey>
```

表示容器属性。

TKey : 属性值的类型。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GenericProperty()](#GenericProperty--) | 初始化 GenericProperty&lt;T&gt; 类的新实例。 |
| [GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name)](#GenericProperty-java.lang.Class-TKey--java.lang.String-) | 初始化 GenericProperty&lt;TKey&gt; 结构的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [&lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2)](#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--) | 返回一个值，指示指定的 `obj1` 实例是否等于指定的 `obj2` 实例。 |
| [Clone()](#Clone--) | 创建并返回此实例的深拷贝。 |
| [CloneTo(GenericProperty&lt;TKey&gt; that)](#CloneTo-com.aspose.tasks.GenericProperty-TKey--) | 将实例的深拷贝复制到另一个实例。 |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getName()](#getName--) | 获取属性的名称。 |
| [getValue()](#getValue--) | 获取属性的值。 |
### GenericProperty() {#GenericProperty--}
```
public GenericProperty()
```


初始化 GenericProperty&lt;T&gt; 类的新实例。

### GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name) {#GenericProperty-java.lang.Class-TKey--java.lang.String-}
```
public GenericProperty(Class<TKey> typeOfTKey, String name)
```


初始化 GenericProperty&lt;TKey&gt; 结构的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| typeOfTKey | java.lang.Class&lt;TKey&gt; |  |
| name | java.lang.String | 属性的名称。 |

### &lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2) {#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--}
```
public static boolean <TKey>equals(GenericProperty<TKey> obj1, GenericProperty<TKey> obj2)
```


返回一个值，指示指定的 `obj1` 实例是否等于指定的 `obj2` 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj1 | [GenericProperty](../../com.aspose.tasks/genericproperty) | 要比较的第一个对象。 |
| obj2 | [GenericProperty](../../com.aspose.tasks/genericproperty) | 要比较的第二个对象。 |

**Returns:**
boolean - 如果指定的 `obj1` 实例等于指定的 `obj2` 实例则返回 true；否则返回 false。
### Clone() {#Clone--}
```
public GenericProperty<TKey> Clone()
```


创建并返回此实例的深拷贝。

**Returns:**
[GenericProperty](../../com.aspose.tasks/genericproperty) - a deep copy of this object.
### CloneTo(GenericProperty&lt;TKey&gt; that) {#CloneTo-com.aspose.tasks.GenericProperty-TKey--}
```
public void CloneTo(GenericProperty<TKey> that)
```


将实例的深拷贝复制到另一个实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| that | [GenericProperty](../../com.aspose.tasks/genericproperty) | 另一个实例。 |

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object | \{@inheritDoc\} |

**Returns:**
布尔 - \{@inheritDoc\}
### getName() {#getName--}
```
public final String getName()
```


获取属性的名称。

**Returns:**
java.lang.String - 属性的名称。
### getValue() {#getValue--}
```
public final Object getValue()
```


获取属性的值。

**Returns:**
java.lang.Object - 属性的值。
