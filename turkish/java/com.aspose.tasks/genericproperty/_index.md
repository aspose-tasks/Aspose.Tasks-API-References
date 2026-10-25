---
title: "GenericProperty"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bir konteyner özelliğini temsil eder."
type: docs
weight: 113
url: /tr/java/com.aspose.tasks/genericproperty/
---

**Inheritance:**
java.lang.Object
```
public class GenericProperty<TKey>
```

Bir konteyner özelliğini temsil eder.

TKey : Özellik değerinin tipi.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [GenericProperty()](#GenericProperty--) | GenericProperty&lt;T&gt; sınıfının yeni bir örneğini başlatır. |
| [GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name)](#GenericProperty-java.lang.Class-TKey--java.lang.String-) | GenericProperty&lt;TKey&gt; yapısının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [&lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2)](#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--) | Belirtilen `obj1` örneğinin belirtilen `obj2` örneğiyle eşit olup olmadığını gösteren bir değer döndürür. |
| [Clone()](#Clone--) | Bu örneğin derin bir kopyasını oluşturur ve döndürür. |
| [CloneTo(GenericProperty&lt;TKey&gt; that)](#CloneTo-com.aspose.tasks.GenericProperty-TKey--) | Örneğin derin bir kopyasını başka bir örneğe yapar. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getName()](#getName--) | Özelliğin adını alır. |
| [getValue()](#getValue--) | Özelliğin değerini alır. |
### GenericProperty() {#GenericProperty--}
```
public GenericProperty()
```


GenericProperty&lt;T&gt; sınıfının yeni bir örneğini başlatır.

### GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name) {#GenericProperty-java.lang.Class-TKey--java.lang.String-}
```
public GenericProperty(Class<TKey> typeOfTKey, String name)
```


GenericProperty&lt;TKey&gt; yapısının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| typeOfTKey | java.lang.Class&lt;TKey&gt; |  |
| name | java.lang.String | Özelliğin adı. |

### &lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2) {#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--}
```
public static boolean <TKey>equals(GenericProperty<TKey> obj1, GenericProperty<TKey> obj2)
```


Belirtilen `obj1` örneğinin belirtilen `obj2` örneğiyle eşit olup olmadığını gösteren bir değer döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj1 | [GenericProperty](../../com.aspose.tasks/genericproperty) | karşılaştırılacak ilk nesne. |
| obj2 | [GenericProperty](../../com.aspose.tasks/genericproperty) | karşılaştırılacak ikinci nesne. |

**Returns:**
boolean - belirtilen `obj1` örneği belirtilen `obj2` örneğine eşitse true döndürür; aksi takdirde false.
### Clone() {#Clone--}
```
public GenericProperty<TKey> Clone()
```


Bu örneğin derin bir kopyasını oluşturur ve döndürür.

**Returns:**
[GenericProperty](../../com.aspose.tasks/genericproperty) - a deep copy of this object.
### CloneTo(GenericProperty&lt;TKey&gt; that) {#CloneTo-com.aspose.tasks.GenericProperty-TKey--}
```
public void CloneTo(GenericProperty<TKey> that)
```


Örneğin derin bir kopyasını başka bir örneğe yapar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| that | [GenericProperty](../../com.aspose.tasks/genericproperty) | başka bir örnek. |

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### getName() {#getName--}
```
public final String getName()
```


Özelliğin adını alır.

**Returns:**
java.lang.String - özelliğin adı.
### getValue() {#getValue--}
```
public final Object getValue()
```


Özelliğin değerini alır.

**Returns:**
java.lang.Object - özelliğin değeri.
