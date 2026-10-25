---
title: "GenericProperty"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Container‑Eigenschaft dar."
type: docs
weight: 113
url: /de/java/com.aspose.tasks/genericproperty/
---

**Inheritance:**
java.lang.Object
```
public class GenericProperty<TKey>
```

Stellt eine Container‑Eigenschaft dar.

TKey : Der Typ des Eigenschaftswerts.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [GenericProperty()](#GenericProperty--) | Initialisiert eine neue Instanz der Klasse GenericProperty&lt;T&gt;. |
| [GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name)](#GenericProperty-java.lang.Class-TKey--java.lang.String-) | Initialisiert eine neue Instanz der Struktur GenericProperty&lt;TKey&gt;. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [&lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2)](#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--) | Gibt einen Wert zurück, der angibt, ob die angegebene `obj1`-Instanz gleich der angegebenen `obj2`-Instanz ist. |
| [Clone()](#Clone--) | Erstellt und gibt eine tiefe Kopie dieser Instanz zurück. |
| [CloneTo(GenericProperty&lt;TKey&gt; that)](#CloneTo-com.aspose.tasks.GenericProperty-TKey--) | Erstellt eine tiefe Kopie der Instanz in einer anderen Instanz. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getName()](#getName--) | Liefert den Namen der Eigenschaft. |
| [getValue()](#getValue--) | Liefert den Wert der Eigenschaft. |
### GenericProperty() {#GenericProperty--}
```
public GenericProperty()
```


Initialisiert eine neue Instanz der Klasse GenericProperty&lt;T&gt;.

### GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name) {#GenericProperty-java.lang.Class-TKey--java.lang.String-}
```
public GenericProperty(Class<TKey> typeOfTKey, String name)
```


Initialisiert eine neue Instanz der Struktur GenericProperty&lt;TKey&gt;.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| typeOfTKey | java.lang.Class&lt;TKey&gt; |  |
| name | java.lang.String | Der Name der Eigenschaft. |

### &lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2) {#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--}
```
public static boolean <TKey>equals(GenericProperty<TKey> obj1, GenericProperty<TKey> obj2)
```


Gibt einen Wert zurück, der angibt, ob die angegebene `obj1`-Instanz gleich der angegebenen `obj2`-Instanz ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj1 | [GenericProperty](../../com.aspose.tasks/genericproperty) | das erste zu vergleichende Objekt. |
| obj2 | [GenericProperty](../../com.aspose.tasks/genericproperty) | das zweite zu vergleichende Objekt. |

**Returns:**
boolean - gibt true zurück, wenn die angegebene `obj1`-Instanz gleich der angegebenen `obj2`-Instanz ist; andernfalls false.
### Clone() {#Clone--}
```
public GenericProperty<TKey> Clone()
```


Erstellt und gibt eine tiefe Kopie dieser Instanz zurück.

**Returns:**
[GenericProperty](../../com.aspose.tasks/genericproperty) - a deep copy of this object.
### CloneTo(GenericProperty&lt;TKey&gt; that) {#CloneTo-com.aspose.tasks.GenericProperty-TKey--}
```
public void CloneTo(GenericProperty<TKey> that)
```


Erstellt eine tiefe Kopie der Instanz in einer anderen Instanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| that | [GenericProperty](../../com.aspose.tasks/genericproperty) | eine andere Instanz. |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \\{@inheritDoc\\}
### getName() {#getName--}
```
public final String getName()
```


Liefert den Namen der Eigenschaft.

**Returns:**
java.lang.String - ein Name der Eigenschaft.
### getValue() {#getValue--}
```
public final Object getValue()
```


Liefert den Wert der Eigenschaft.

**Returns:**
java.lang.Object - ein Wert der Eigenschaft.
