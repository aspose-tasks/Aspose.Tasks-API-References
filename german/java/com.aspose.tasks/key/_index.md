---
title: "Key"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt einen Eigenschaftsschlüssel einer Klasse des angegebenen Typs dar."
type: docs
weight: 139
url: /de/java/com.aspose.tasks/key/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct
```
public class Key<T,K> extends Struct<Key<T,K>>
```

Stellt einen Eigenschaftsschlüssel einer Klasse des angegebenen Typs dar. Eine Instanz dieser Klasse wird verwendet, wenn eine Eigenschaft eines Containers gelesen oder gesetzt wird.

T : Der Typ des Eigenschaftswerts.
K : Der Typ des Eigenschaftsschlüssels.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [Clone()](#Clone--) | Gibt eine tiefe Kopie der Instanz zurück. |
| [CloneTo(Key&lt;T,K&gt; that)](#CloneTo-com.aspose.tasks.Key-T-K--) | Erstellt eine tiefe Kopie der Instanz in einer anderen Instanz. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Key obj1, Key obj2)](#equals-com.aspose.tasks.Key-com.aspose.tasks.Key-) | Gibt einen Wert zurück, der angibt, ob die angegebene `obj1`-Instanz gleich der angegebenen `obj2`-Instanz ist. |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getKeyType()](#getKeyType--) | Liefert den Schlüssel der Eigenschaft. |
| [hashCode()](#hashCode--) | Gibt einen Hashcode für die Instanz der Klasse Key zurück. |
### Clone() {#Clone--}
```
public Key<T,K> Clone()
```


Gibt eine tiefe Kopie der Instanz zurück.

**Returns:**
[Key](../../com.aspose.tasks/key) - deep copy of the instance.
### CloneTo(Key&lt;T,K&gt; that) {#CloneTo-com.aspose.tasks.Key-T-K--}
```
public void CloneTo(Key<T,K> that)
```


Erstellt eine tiefe Kopie der Instanz in einer anderen Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| that | [Key](../../com.aspose.tasks/key) | eine andere Instanz. |

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


Gibt einen Wert zurück, der angibt, ob die angegebene `obj1`-Instanz gleich der angegebenen `obj2`-Instanz ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj1 | com.aspose.tasks.Key | das erste zu vergleichende Objekt. |
| obj2 | com.aspose.tasks.Key | das zweite zu vergleichende Objekt. |

**Returns:**
boolean - gibt true zurück, wenn die angegebene `obj1`-Instanz gleich der angegebenen `obj2`-Instanz ist; andernfalls false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \\{@inheritDoc\\}
### getKeyType() {#getKeyType--}
```
public final K getKeyType()
```


Liefert den Schlüssel der Eigenschaft.

**Returns:**
K - der Schlüssel der Eigenschaft.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Gibt einen Hashcode für die Instanz der Klasse Key zurück.

**Returns:**
int - gibt einen Hashcode für dieses Objekt zurück.
