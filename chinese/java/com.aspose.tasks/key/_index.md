---
title: "键"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示指定类型的类的属性键。"
type: docs
weight: 139
url: /zh/java/com.aspose.tasks/key/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct
```
public class Key<T,K> extends Struct<Key<T,K>>
```

表示指定类型类的属性键。获取或设置容器属性时使用此类的实例。

T : 属性值的类型。
K : 属性键的类型。
## 方法

| 方法 | 描述 |
| --- | --- |
| [Clone()](#Clone--) | 返回实例的深拷贝。 |
| [CloneTo(Key&lt;T,K&gt; that)](#CloneTo-com.aspose.tasks.Key-T-K--) | 将实例的深拷贝复制到另一个实例。 |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Key obj1, Key obj2)](#equals-com.aspose.tasks.Key-com.aspose.tasks.Key-) | 返回一个值，指示指定的 `obj1` 实例是否等于指定的 `obj2` 实例。 |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getKeyType()](#getKeyType--) | 获取属性的键。 |
| [hashCode()](#hashCode--) | 返回 Key 类实例的哈希码。 |
### Clone() {#Clone--}
```
public Key<T,K> Clone()
```


返回实例的深拷贝。

**Returns:**
[Key](../../com.aspose.tasks/key) - deep copy of the instance.
### CloneTo(Key&lt;T,K&gt; that) {#CloneTo-com.aspose.tasks.Key-T-K--}
```
public void CloneTo(Key<T,K> that)
```


将实例的深拷贝复制到另一个实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| that | [Key](../../com.aspose.tasks/key) | 另一个实例。 |

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


返回一个值，指示指定的 `obj1` 实例是否等于指定的 `obj2` 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj1 | com.aspose.tasks.Key | 要比较的第一个对象。 |
| obj2 | com.aspose.tasks.Key | 要比较的第二个对象。 |

**Returns:**
boolean - 如果指定的 `obj1` 实例等于指定的 `obj2` 实例则返回 true；否则返回 false。
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
### getKeyType() {#getKeyType--}
```
public final K getKeyType()
```


获取属性的键。

**Returns:**
K - 属性的键。
### hashCode() {#hashCode--}
```
public int hashCode()
```


返回 Key 类实例的哈希码。

**Returns:**
int - 返回此对象的哈希码。
