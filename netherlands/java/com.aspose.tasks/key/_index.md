---
title: "Key"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een eigenschaps-sleutel van een klasse van het opgegeven type voor."
type: docs
weight: 139
url: /nl/java/com.aspose.tasks/key/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct
```
public class Key<T,K> extends Struct<Key<T,K>>
```

Stelt een eigenschaps-sleutel van een klasse van het opgegeven type voor. Een instantie van deze klasse wordt gebruikt bij het ophalen of instellen van een eigenschap van een container.

T : Het type van de eigenschapswaarde.
K : Het type van de eigenschapsleutel.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [Clone()](#Clone--) | Retourneert een diepe kopie van de instantie. |
| [CloneTo(Key&lt;T,K&gt; that)](#CloneTo-com.aspose.tasks.Key-T-K--) | Maakt een diepe kopie van het exemplaar naar een ander exemplaar. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Key obj1, Key obj2)](#equals-com.aspose.tasks.Key-com.aspose.tasks.Key-) | Retourneert een waarde die aangeeft of het opgegeven `obj1`-exemplaar gelijk is aan het opgegeven `obj2`-exemplaar. |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getKeyType()](#getKeyType--) | Haalt de sleutel van de eigenschap op. |
| [hashCode()](#hashCode--) | Retourneert een hashcode voor de instantie van de Key-klasse. |
### Clone() {#Clone--}
```
public Key<T,K> Clone()
```


Retourneert een diepe kopie van de instantie.

**Returns:**
[Key](../../com.aspose.tasks/key) - deep copy of the instance.
### CloneTo(Key&lt;T,K&gt; that) {#CloneTo-com.aspose.tasks.Key-T-K--}
```
public void CloneTo(Key<T,K> that)
```


Maakt een diepe kopie van het exemplaar naar een ander exemplaar.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| that | [Key](../../com.aspose.tasks/key) | een andere instantie. |

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


Retourneert een waarde die aangeeft of het opgegeven `obj1`-exemplaar gelijk is aan het opgegeven `obj2`-exemplaar.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj1 | com.aspose.tasks.Key | het eerste object om te vergelijken. |
| obj2 | com.aspose.tasks.Key | het tweede object om te vergelijken. |

**Returns:**
boolean - retourneert true als de opgegeven `obj1`-instantie gelijk is aan de opgegeven `obj2`-instantie; anders false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### getKeyType() {#getKeyType--}
```
public final K getKeyType()
```


Haalt de sleutel van de eigenschap op.

**Returns:**
K - de sleutel van de eigenschap.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Retourneert een hashcode voor de instantie van de Key-klasse.

**Returns:**
int - retourneert een hashcode voor dit object.
