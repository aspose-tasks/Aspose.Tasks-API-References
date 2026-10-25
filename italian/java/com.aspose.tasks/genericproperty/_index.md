---
title: "GenericProperty"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta una proprietà del contenitore."
type: docs
weight: 113
url: /it/java/com.aspose.tasks/genericproperty/
---

**Inheritance:**
java.lang.Object
```
public class GenericProperty<TKey>
```

Rappresenta una proprietà del contenitore.

TKey : Il tipo di valore della proprietà.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [GenericProperty()](#GenericProperty--) | Inizializza una nuova istanza della classe GenericProperty&lt;T&gt;. |
| [GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name)](#GenericProperty-java.lang.Class-TKey--java.lang.String-) | Inizializza una nuova istanza della struct GenericProperty&lt;TKey&gt;. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [&lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2)](#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--) | Restituisce un valore che indica se l'istanza specificata `obj1` è uguale all'istanza specificata `obj2`. |
| [Clone()](#Clone--) | Crea e restituisce una copia profonda di questa istanza. |
| [CloneTo(GenericProperty&lt;TKey&gt; that)](#CloneTo-com.aspose.tasks.GenericProperty-TKey--) | Crea una copia profonda dell'istanza in un'altra istanza. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getName()](#getName--) | Ottiene il nome della proprietà. |
| [getValue()](#getValue--) | Ottiene il valore della proprietà. |
### GenericProperty() {#GenericProperty--}
```
public GenericProperty()
```


Inizializza una nuova istanza della classe GenericProperty&lt;T&gt;.

### GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name) {#GenericProperty-java.lang.Class-TKey--java.lang.String-}
```
public GenericProperty(Class<TKey> typeOfTKey, String name)
```


Inizializza una nuova istanza della struct GenericProperty&lt;TKey&gt;.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| typeOfTKey | java.lang.Class&lt;TKey&gt; |  |
| name | java.lang.String | Il nome della proprietà. |

### &lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2) {#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--}
```
public static boolean <TKey>equals(GenericProperty<TKey> obj1, GenericProperty<TKey> obj2)
```


Restituisce un valore che indica se l'istanza specificata `obj1` è uguale all'istanza specificata `obj2`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj1 | [GenericProperty](../../com.aspose.tasks/genericproperty) | il primo oggetto da confrontare. |
| obj2 | [GenericProperty](../../com.aspose.tasks/genericproperty) | il secondo oggetto da confrontare. |

**Returns:**
boolean - restituisce true se l'istanza specificata `obj1` è uguale all'istanza specificata `obj2`; altrimenti, false.
### Clone() {#Clone--}
```
public GenericProperty<TKey> Clone()
```


Crea e restituisce una copia profonda di questa istanza.

**Returns:**
[GenericProperty](../../com.aspose.tasks/genericproperty) - a deep copy of this object.
### CloneTo(GenericProperty&lt;TKey&gt; that) {#CloneTo-com.aspose.tasks.GenericProperty-TKey--}
```
public void CloneTo(GenericProperty<TKey> that)
```


Crea una copia profonda dell'istanza in un'altra istanza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| that | [GenericProperty](../../com.aspose.tasks/genericproperty) | un'altra istanza. |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### getName() {#getName--}
```
public final String getName()
```


Ottiene il nome della proprietà.

**Returns:**
java.lang.String - un nome della proprietà.
### getValue() {#getValue--}
```
public final Object getValue()
```


Ottiene il valore della proprietà.

**Returns:**
java.lang.Object - un valore della proprietà.
