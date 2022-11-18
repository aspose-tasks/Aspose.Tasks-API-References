---
title: Key
second_title: Aspose.Tasks for Java API Reference
description: Represents a property key of a class of the specified type.
type: docs
weight: 132
url: /java/com.aspose.tasks/key/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct
```
public class Key<T,K> extends Struct<Key<T,K>>
```

Represents a property key of a class of the specified type. An instance of this class is used when getting or setting property of a container.

 T : The type of property value.
 K : The type of property key.
## Methods

| Method | Description |
| --- | --- |
| [Clone()](#Clone--) | Returns deep copy of the instance. |
| [CloneTo(Key&lt;T,K&gt; that)](#CloneTo-com.aspose.tasks.Key-T-K--) | Makes a deep copy of the instance into another instance. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Key obj1, Key obj2)](#equals-com.aspose.tasks.Key-com.aspose.tasks.Key-) | Returns a value indicating whether specified  obj1  instance is equal to the specified  obj2  instance. |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getKeyType()](#getKeyType--) | Gets the key of the property. |
| [hashCode()](#hashCode--) | Returns a hash code for the instance of the Key class. |
### Clone() {#Clone--}
```
public Key<T,K> Clone()
```


Returns deep copy of the instance.

**Returns:**
[Key](../../com.aspose.tasks/key) - deep copy of the instance.
### CloneTo(Key&lt;T,K&gt; that) {#CloneTo-com.aspose.tasks.Key-T-K--}
```
public void CloneTo(Key<T,K> that)
```


Makes a deep copy of the instance into another instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| that | [Key](../../com.aspose.tasks/key) | another instance. |

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


Returns a value indicating whether specified  obj1  instance is equal to the specified  obj2  instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj1 | com.aspose.tasks.Key | the first object to compare. |
| obj2 | com.aspose.tasks.Key | the second object to compare. |

**Returns:**
boolean - returns true if specified  obj1  instance is equal to the specified  obj2  instance; otherwise, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### getKeyType() {#getKeyType--}
```
public final K getKeyType()
```


Gets the key of the property.

**Returns:**
K - the key of the property.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returns a hash code for the instance of the Key class.

**Returns:**
int - returns a hash code for this object.
