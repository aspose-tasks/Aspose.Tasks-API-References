---
title: "Key"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una clave de propiedad de una clase del tipo especificado."
type: docs
weight: 139
url: /es/java/com.aspose.tasks/key/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct
```
public class Key<T,K> extends Struct<Key<T,K>>
```

Representa una clave de propiedad de una clase del tipo especificado. Una instancia de esta clase se utiliza al obtener o establecer una propiedad de un contenedor.

T : El tipo del valor de la propiedad.
K : El tipo de la clave de la propiedad.
## Métodos

| Método | Descripción |
| --- | --- |
| [Clone()](#Clone--) | Devuelve una copia profunda de la instancia. |
| [CloneTo(Key&lt;T,K&gt; that)](#CloneTo-com.aspose.tasks.Key-T-K--) | Realiza una copia profunda de la instancia en otra instancia. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Key obj1, Key obj2)](#equals-com.aspose.tasks.Key-com.aspose.tasks.Key-) | Devuelve un valor que indica si la instancia `obj1` especificada es igual a la instancia `obj2` especificada. |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getKeyType()](#getKeyType--) | Obtiene la clave de la propiedad. |
| [hashCode()](#hashCode--) | Devuelve un código hash para la instancia de la clase Key. |
### Clone() {#Clone--}
```
public Key<T,K> Clone()
```


Devuelve una copia profunda de la instancia.

**Returns:**
[Key](../../com.aspose.tasks/key) - deep copy of the instance.
### CloneTo(Key&lt;T,K&gt; that) {#CloneTo-com.aspose.tasks.Key-T-K--}
```
public void CloneTo(Key<T,K> that)
```


Realiza una copia profunda de la instancia en otra instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| that | [Key](../../com.aspose.tasks/key) | otra instancia. |

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


Devuelve un valor que indica si la instancia `obj1` especificada es igual a la instancia `obj2` especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj1 | com.aspose.tasks.Key | el primer objeto a comparar. |
| obj2 | com.aspose.tasks.Key | el segundo objeto a comparar. |

**Returns:**
boolean - devuelve true si la instancia especificada `obj1` es igual a la instancia especificada `obj2`; de lo contrario, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### getKeyType() {#getKeyType--}
```
public final K getKeyType()
```


Obtiene la clave de la propiedad.

**Returns:**
K - la clave de la propiedad.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Devuelve un código hash para la instancia de la clase Key.

**Returns:**
int - devuelve un código hash para este objeto.
