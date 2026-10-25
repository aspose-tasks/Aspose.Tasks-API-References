---
title: "GenericProperty"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une propriété de conteneur."
type: docs
weight: 113
url: /fr/java/com.aspose.tasks/genericproperty/
---

**Inheritance:**
java.lang.Object
```
public class GenericProperty<TKey>
```

Représente une propriété de conteneur.

TKey : Le type de valeur de propriété.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [GenericProperty()](#GenericProperty--) | Initialise une nouvelle instance de la classe GenericProperty&lt;T&gt;. |
| [GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name)](#GenericProperty-java.lang.Class-TKey--java.lang.String-) | Initialise une nouvelle instance de la structure GenericProperty&lt;TKey&gt;. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [&lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2)](#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--) | Renvoie une valeur indiquant si l'instance `obj1` spécifiée est égale à l'instance `obj2` spécifiée. |
| [Clone()](#Clone--) | Crée et renvoie une copie profonde de cette instance. |
| [CloneTo(GenericProperty&lt;TKey&gt; that)](#CloneTo-com.aspose.tasks.GenericProperty-TKey--) | Effectue une copie profonde de l'instance dans une autre instance. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getName()](#getName--) | Obtient le nom de la propriété. |
| [getValue()](#getValue--) | Obtient la valeur de la propriété. |
### GenericProperty() {#GenericProperty--}
```
public GenericProperty()
```


Initialise une nouvelle instance de la classe GenericProperty&lt;T&gt;.

### GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name) {#GenericProperty-java.lang.Class-TKey--java.lang.String-}
```
public GenericProperty(Class<TKey> typeOfTKey, String name)
```


Initialise une nouvelle instance de la structure GenericProperty&lt;TKey&gt;.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| typeOfTKey | java.lang.Class&lt;TKey&gt; |  |
| name | java.lang.String | Le nom de la propriété. |

### &lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2) {#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--}
```
public static boolean <TKey>equals(GenericProperty<TKey> obj1, GenericProperty<TKey> obj2)
```


Renvoie une valeur indiquant si l'instance `obj1` spécifiée est égale à l'instance `obj2` spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj1 | [GenericProperty](../../com.aspose.tasks/genericproperty) | le premier objet à comparer. |
| obj2 | [GenericProperty](../../com.aspose.tasks/genericproperty) | le deuxième objet à comparer. |

**Returns:**
boolean - renvoie true si l'instance `obj1` spécifiée est égale à l'instance `obj2` spécifiée ; sinon, false.
### Clone() {#Clone--}
```
public GenericProperty<TKey> Clone()
```


Crée et renvoie une copie profonde de cette instance.

**Returns:**
[GenericProperty](../../com.aspose.tasks/genericproperty) - a deep copy of this object.
### CloneTo(GenericProperty&lt;TKey&gt; that) {#CloneTo-com.aspose.tasks.GenericProperty-TKey--}
```
public void CloneTo(GenericProperty<TKey> that)
```


Effectue une copie profonde de l'instance dans une autre instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| that | [GenericProperty](../../com.aspose.tasks/genericproperty) | une autre instance. |

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
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | \{@inheritDoc\} |

**Returns:**
booléen - \{@inheritDoc\}
### getName() {#getName--}
```
public final String getName()
```


Obtient le nom de la propriété.

**Returns:**
java.lang.String - un nom de la propriété.
### getValue() {#getValue--}
```
public final Object getValue()
```


Obtient la valeur de la propriété.

**Returns:**
java.lang.Object - une valeur de la propriété.
