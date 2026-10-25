---
title: "GenericProperty"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een container‑eigenschap voor."
type: docs
weight: 113
url: /nl/java/com.aspose.tasks/genericproperty/
---

**Inheritance:**
java.lang.Object
```
public class GenericProperty<TKey>
```

Stelt een container‑eigenschap voor.

TKey : Het type van de eigenschapswaarde.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [GenericProperty()](#GenericProperty--) | Initialiseert een nieuw exemplaar van de GenericProperty&lt;T&gt; klasse. |
| [GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name)](#GenericProperty-java.lang.Class-TKey--java.lang.String-) | Initialiseert een nieuw exemplaar van de GenericProperty&lt;TKey&gt; struct. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [&lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2)](#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--) | Retourneert een waarde die aangeeft of het opgegeven `obj1`-exemplaar gelijk is aan het opgegeven `obj2`-exemplaar. |
| [Clone()](#Clone--) | Maakt en retourneert een diepe kopie van dit exemplaar. |
| [CloneTo(GenericProperty&lt;TKey&gt; that)](#CloneTo-com.aspose.tasks.GenericProperty-TKey--) | Maakt een diepe kopie van het exemplaar naar een ander exemplaar. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getName()](#getName--) | Haalt de naam van de eigenschap op. |
| [getValue()](#getValue--) | Haalt de waarde van de eigenschap op. |
### GenericProperty() {#GenericProperty--}
```
public GenericProperty()
```


Initialiseert een nieuw exemplaar van de GenericProperty&lt;T&gt; klasse.

### GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name) {#GenericProperty-java.lang.Class-TKey--java.lang.String-}
```
public GenericProperty(Class<TKey> typeOfTKey, String name)
```


Initialiseert een nieuw exemplaar van de GenericProperty&lt;TKey&gt; struct.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| typeOfTKey | java.lang.Class&lt;TKey&gt; |  |
| naam | java.lang.String | De naam van de eigenschap. |

### &lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2) {#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--}
```
public static boolean <TKey>equals(GenericProperty<TKey> obj1, GenericProperty<TKey> obj2)
```


Retourneert een waarde die aangeeft of het opgegeven `obj1`-exemplaar gelijk is aan het opgegeven `obj2`-exemplaar.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj1 | [GenericProperty](../../com.aspose.tasks/genericproperty) | het eerste object om te vergelijken. |
| obj2 | [GenericProperty](../../com.aspose.tasks/genericproperty) | het tweede object om te vergelijken. |

**Returns:**
boolean - retourneert true als de opgegeven `obj1`-instantie gelijk is aan de opgegeven `obj2`-instantie; anders false.
### Clone() {#Clone--}
```
public GenericProperty<TKey> Clone()
```


Maakt en retourneert een diepe kopie van dit exemplaar.

**Returns:**
[GenericProperty](../../com.aspose.tasks/genericproperty) - a deep copy of this object.
### CloneTo(GenericProperty&lt;TKey&gt; that) {#CloneTo-com.aspose.tasks.GenericProperty-TKey--}
```
public void CloneTo(GenericProperty<TKey> that)
```


Maakt een diepe kopie van het exemplaar naar een ander exemplaar.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| that | [GenericProperty](../../com.aspose.tasks/genericproperty) | een andere instantie. |

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### getName() {#getName--}
```
public final String getName()
```


Haalt de naam van de eigenschap op.

**Returns:**
java.lang.String - een naam van de eigenschap.
### getValue() {#getValue--}
```
public final Object getValue()
```


Haalt de waarde van de eigenschap op.

**Returns:**
java.lang.Object - een waarde van de eigenschap.
