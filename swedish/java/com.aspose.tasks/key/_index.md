---
title: "Key"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en egenskapsnyckel för en klass av den angivna typen."
type: docs
weight: 139
url: /sv/java/com.aspose.tasks/key/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct
```
public class Key<T,K> extends Struct<Key<T,K>>
```

Representerar en egenskapsnyckel för en klass av den angivna typen. En instans av denna klass används när egenskapen för en behållare hämtas eller sätts.

T : Typen av egenskapsvärde.
K : Typen av egenskapsnyckel.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [Clone()](#Clone--) | Returnerar en djup kopia av instansen. |
| [CloneTo(Key&lt;T,K&gt; that)](#CloneTo-com.aspose.tasks.Key-T-K--) | Gör en djup kopia av instansen till en annan instans. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Key obj1, Key obj2)](#equals-com.aspose.tasks.Key-com.aspose.tasks.Key-) | Returnerar ett värde som indikerar om den angivna `obj1`-instansen är lika med den angivna `obj2`-instansen. |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getKeyType()](#getKeyType--) | Hämtar nyckeln för egenskapen. |
| [hashCode()](#hashCode--) | Returnerar en hashkod för instansen av klassen Key. |
### Clone() {#Clone--}
```
public Key<T,K> Clone()
```


Returnerar en djup kopia av instansen.

**Returns:**
[Key](../../com.aspose.tasks/key) - deep copy of the instance.
### CloneTo(Key&lt;T,K&gt; that) {#CloneTo-com.aspose.tasks.Key-T-K--}
```
public void CloneTo(Key<T,K> that)
```


Gör en djup kopia av instansen till en annan instans.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| that | [Key](../../com.aspose.tasks/key) | annan instans. |

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


Returnerar ett värde som indikerar om den angivna `obj1`-instansen är lika med den angivna `obj2`-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj1 | com.aspose.tasks.Key | det första objektet att jämföra. |
| obj2 | com.aspose.tasks.Key | det andra objektet att jämföra. |

**Returns:**
boolean - returnerar true om den specificerade `obj1`-instansen är lika med den specificerade `obj2`-instansen; annars false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### getKeyType() {#getKeyType--}
```
public final K getKeyType()
```


Hämtar nyckeln för egenskapen.

**Returns:**
K - nyckeln för egenskapen.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returnerar en hashkod för instansen av klassen Key.

**Returns:**
int - returnerar en hashkod för detta objekt.
