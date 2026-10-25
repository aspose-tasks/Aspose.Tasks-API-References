---
title: "Key"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Belirtilen türde bir sınıfın özellik anahtarını temsil eder."
type: docs
weight: 139
url: /tr/java/com.aspose.tasks/key/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct
```
public class Key<T,K> extends Struct<Key<T,K>>
```

Belirtilen türde bir sınıfın özellik anahtarını temsil eder. Bu sınıfın bir örneği, bir kapsayıcının özelliğini alırken veya ayarlarken kullanılır.

T : Özellik değerinin türü.
K : Özellik anahtarının türü.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [Clone()](#Clone--) | Örneğin derin kopyasını döndürür. |
| [CloneTo(Key&lt;T,K&gt; that)](#CloneTo-com.aspose.tasks.Key-T-K--) | Örneğin derin bir kopyasını başka bir örneğe yapar. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Key obj1, Key obj2)](#equals-com.aspose.tasks.Key-com.aspose.tasks.Key-) | Belirtilen `obj1` örneğinin belirtilen `obj2` örneğiyle eşit olup olmadığını gösteren bir değer döndürür. |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getKeyType()](#getKeyType--) | Özelliğin anahtarını alır. |
| [hashCode()](#hashCode--) | Key sınıfının örneği için bir karma kodu döndürür. |
### Clone() {#Clone--}
```
public Key<T,K> Clone()
```


Örneğin derin kopyasını döndürür.

**Returns:**
[Key](../../com.aspose.tasks/key) - deep copy of the instance.
### CloneTo(Key&lt;T,K&gt; that) {#CloneTo-com.aspose.tasks.Key-T-K--}
```
public void CloneTo(Key<T,K> that)
```


Örneğin derin bir kopyasını başka bir örneğe yapar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| that | [Key](../../com.aspose.tasks/key) | başka bir örnek. |

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


Belirtilen `obj1` örneğinin belirtilen `obj2` örneğiyle eşit olup olmadığını gösteren bir değer döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj1 | com.aspose.tasks.Key | karşılaştırılacak ilk nesne. |
| obj2 | com.aspose.tasks.Key | karşılaştırılacak ikinci nesne. |

**Returns:**
boolean - belirtilen `obj1` örneği belirtilen `obj2` örneğine eşitse true döndürür; aksi takdirde false.
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
### getKeyType() {#getKeyType--}
```
public final K getKeyType()
```


Özelliğin anahtarını alır.

**Returns:**
K - özelliğin anahtarı.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Key sınıfının örneği için bir karma kodu döndürür.

**Returns:**
int - bu nesne için bir karma kodu döndürür.
