---
title: GenericProperty
second_title: Aspose.Tasks for Java API Reference
description: Represents a container property.
type: docs
weight: 112
url: /java/com.aspose.tasks/genericproperty/
---

**Inheritance:**
java.lang.Object
```
public class GenericProperty<TKey>
```

Represents a container property.

 TKey : The type of property value.
## Constructors

| Constructor | Description |
| --- | --- |
| [GenericProperty()](#GenericProperty--) | Initializes a new instance of the GenericProperty&lt;T&gt; class. |
| [GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name)](#GenericProperty-java.lang.Class-TKey--java.lang.String-) | Initializes a new instance of the GenericProperty&lt;TKey&gt; struct. |
## Methods

| Method | Description |
| --- | --- |
| [&lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2)](#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--) | Returns a value indicating whether specified  obj1  instance is equal to the specified  obj2  instance. |
| [Clone()](#Clone--) | Creates and returns a deep copy of this instance. |
| [CloneTo(GenericProperty&lt;TKey&gt; that)](#CloneTo-com.aspose.tasks.GenericProperty-TKey--) | Makes a deep copy of the instance into another instance. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getName()](#getName--) | Gets a name of the property. |
| [getValue()](#getValue--) | Gets a value of the property. |
### GenericProperty() {#GenericProperty--}
```
public GenericProperty()
```


Initializes a new instance of the GenericProperty&lt;T&gt; class.

### GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name) {#GenericProperty-java.lang.Class-TKey--java.lang.String-}
```
public GenericProperty(Class<TKey> typeOfTKey, String name)
```


Initializes a new instance of the GenericProperty&lt;TKey&gt; struct.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| typeOfTKey | java.lang.Class&lt;TKey&gt; |  |
| name | java.lang.String | The name of the property. |

### &lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2) {#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--}
```
public static boolean <TKey>equals(GenericProperty<TKey> obj1, GenericProperty<TKey> obj2)
```


Returns a value indicating whether specified  obj1  instance is equal to the specified  obj2  instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj1 | [GenericProperty](../../com.aspose.tasks/genericproperty) | the first object to compare. |
| obj2 | [GenericProperty](../../com.aspose.tasks/genericproperty) | the second object to compare. |

**Returns:**
boolean - returns true if specified  obj1  instance is equal to the specified  obj2  instance; otherwise, false.
### Clone() {#Clone--}
```
public GenericProperty<TKey> Clone()
```


Creates and returns a deep copy of this instance.

**Returns:**
[GenericProperty](../../com.aspose.tasks/genericproperty) - a deep copy of this object.
### CloneTo(GenericProperty&lt;TKey&gt; that) {#CloneTo-com.aspose.tasks.GenericProperty-TKey--}
```
public void CloneTo(GenericProperty<TKey> that)
```


Makes a deep copy of the instance into another instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| that | [GenericProperty](../../com.aspose.tasks/genericproperty) | another instance. |

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
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### getName() {#getName--}
```
public final String getName()
```


Gets a name of the property.

**Returns:**
java.lang.String - a name of the property.
### getValue() {#getValue--}
```
public final Object getValue()
```


Gets a value of the property.

**Returns:**
java.lang.Object - a value of the property.
