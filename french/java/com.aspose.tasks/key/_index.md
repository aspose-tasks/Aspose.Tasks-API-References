---
title: "Key"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une clé de propriété d'une classe du type spécifié."
type: docs
weight: 139
url: /fr/java/com.aspose.tasks/key/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct
```
public class Key<T,K> extends Struct<Key<T,K>>
```

Représente une clé de propriété d'une classe du type spécifié. Une instance de cette classe est utilisée lors de la lecture ou de l'écriture d'une propriété d'un conteneur.

T : Le type de la valeur de la propriété.
K : Le type de la clé de la propriété.
## Méthodes

| Méthode | Description |
| --- | --- |
| [Clone()](#Clone--) | Renvoie une copie profonde de l'instance. |
| [CloneTo(Key&lt;T,K&gt; that)](#CloneTo-com.aspose.tasks.Key-T-K--) | Effectue une copie profonde de l'instance dans une autre instance. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Key obj1, Key obj2)](#equals-com.aspose.tasks.Key-com.aspose.tasks.Key-) | Renvoie une valeur indiquant si l'instance `obj1` spécifiée est égale à l'instance `obj2` spécifiée. |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getKeyType()](#getKeyType--) | Obtient la clé de la propriété. |
| [hashCode()](#hashCode--) | Renvoie un code de hachage pour l'instance de la classe Key. |
### Clone() {#Clone--}
```
public Key<T,K> Clone()
```


Renvoie une copie profonde de l'instance.

**Returns:**
[Key](../../com.aspose.tasks/key) - deep copy of the instance.
### CloneTo(Key&lt;T,K&gt; that) {#CloneTo-com.aspose.tasks.Key-T-K--}
```
public void CloneTo(Key<T,K> that)
```


Effectue une copie profonde de l'instance dans une autre instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| that | [Key](../../com.aspose.tasks/key) | une autre instance. |

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


Renvoie une valeur indiquant si l'instance `obj1` spécifiée est égale à l'instance `obj2` spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj1 | com.aspose.tasks.Key | le premier objet à comparer. |
| obj2 | com.aspose.tasks.Key | le deuxième objet à comparer. |

**Returns:**
boolean - renvoie true si l'instance `obj1` spécifiée est égale à l'instance `obj2` spécifiée ; sinon, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | \{@inheritDoc\} |

**Returns:**
booléen - \{@inheritDoc\}
### getKeyType() {#getKeyType--}
```
public final K getKeyType()
```


Obtient la clé de la propriété.

**Returns:**
K - la clé de la propriété.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Renvoie un code de hachage pour l'instance de la classe Key.

**Returns:**
int - renvoie un code de hachage pour cet objet.
