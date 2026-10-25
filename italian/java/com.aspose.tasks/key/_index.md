---
title: "Key"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta una chiave di proprietà di una classe del tipo specificato."
type: docs
weight: 139
url: /it/java/com.aspose.tasks/key/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct
```
public class Key<T,K> extends Struct<Key<T,K>>
```

Rappresenta una chiave di proprietà di una classe del tipo specificato. Un'istanza di questa classe viene utilizzata quando si ottiene o si imposta una proprietà di un contenitore.

T : Il tipo del valore della proprietà.
K : Il tipo della chiave della proprietà.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [Clone()](#Clone--) | Restituisce una copia profonda dell'istanza. |
| [CloneTo(Key&lt;T,K&gt; that)](#CloneTo-com.aspose.tasks.Key-T-K--) | Crea una copia profonda dell'istanza in un'altra istanza. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Key obj1, Key obj2)](#equals-com.aspose.tasks.Key-com.aspose.tasks.Key-) | Restituisce un valore che indica se l'istanza specificata `obj1` è uguale all'istanza specificata `obj2`. |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getKeyType()](#getKeyType--) | Ottiene la chiave della proprietà. |
| [hashCode()](#hashCode--) | Restituisce un codice hash per l'istanza della classe Key. |
### Clone() {#Clone--}
```
public Key<T,K> Clone()
```


Restituisce una copia profonda dell'istanza.

**Returns:**
[Key](../../com.aspose.tasks/key) - deep copy of the instance.
### CloneTo(Key&lt;T,K&gt; that) {#CloneTo-com.aspose.tasks.Key-T-K--}
```
public void CloneTo(Key<T,K> that)
```


Crea una copia profonda dell'istanza in un'altra istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| that | [Key](../../com.aspose.tasks/key) | un'altra istanza. |

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


Restituisce un valore che indica se l'istanza specificata `obj1` è uguale all'istanza specificata `obj2`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj1 | com.aspose.tasks.Key | il primo oggetto da confrontare. |
| obj2 | com.aspose.tasks.Key | il secondo oggetto da confrontare. |

**Returns:**
boolean - restituisce true se l'istanza specificata `obj1` è uguale all'istanza specificata `obj2`; altrimenti, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### getKeyType() {#getKeyType--}
```
public final K getKeyType()
```


Ottiene la chiave della proprietà.

**Returns:**
K - la chiave della proprietà.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Restituisce un codice hash per l'istanza della classe Key.

**Returns:**
int - restituisce un codice hash per questo oggetto.
