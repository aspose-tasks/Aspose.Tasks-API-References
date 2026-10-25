---
title: "GenericProperty"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en containeregenskap."
type: docs
weight: 113
url: /sv/java/com.aspose.tasks/genericproperty/
---

**Inheritance:**
java.lang.Object
```
public class GenericProperty<TKey>
```

Representerar en containeregenskap.

TKey : Typen av egenskapsvärde.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [GenericProperty()](#GenericProperty--) | Initierar en ny instans av klassen GenericProperty&lt;T&gt;. |
| [GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name)](#GenericProperty-java.lang.Class-TKey--java.lang.String-) | Initierar en ny instans av strukturen GenericProperty&lt;TKey&gt;. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [&lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2)](#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--) | Returnerar ett värde som indikerar om den angivna `obj1`-instansen är lika med den angivna `obj2`-instansen. |
| [Clone()](#Clone--) | Skapar och returnerar en djup kopia av denna instans. |
| [CloneTo(GenericProperty&lt;TKey&gt; that)](#CloneTo-com.aspose.tasks.GenericProperty-TKey--) | Gör en djup kopia av instansen till en annan instans. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getName()](#getName--) | Hämtar ett namn på egenskapen. |
| [getValue()](#getValue--) | Hämtar ett värde på egenskapen. |
### GenericProperty() {#GenericProperty--}
```
public GenericProperty()
```


Initierar en ny instans av klassen GenericProperty&lt;T&gt;.

### GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name) {#GenericProperty-java.lang.Class-TKey--java.lang.String-}
```
public GenericProperty(Class<TKey> typeOfTKey, String name)
```


Initierar en ny instans av strukturen GenericProperty&lt;TKey&gt;.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typeOfTKey | java.lang.Class&lt;TKey&gt; |  |
| name | java.lang.String | Namnet på egenskapen. |

### &lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2) {#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--}
```
public static boolean <TKey>equals(GenericProperty<TKey> obj1, GenericProperty<TKey> obj2)
```


Returnerar ett värde som indikerar om den angivna `obj1`-instansen är lika med den angivna `obj2`-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj1 | [GenericProperty](../../com.aspose.tasks/genericproperty) | det första objektet att jämföra. |
| obj2 | [GenericProperty](../../com.aspose.tasks/genericproperty) | det andra objektet att jämföra. |

**Returns:**
boolean - returnerar true om den specificerade `obj1`-instansen är lika med den specificerade `obj2`-instansen; annars false.
### Clone() {#Clone--}
```
public GenericProperty<TKey> Clone()
```


Skapar och returnerar en djup kopia av denna instans.

**Returns:**
[GenericProperty](../../com.aspose.tasks/genericproperty) - a deep copy of this object.
### CloneTo(GenericProperty&lt;TKey&gt; that) {#CloneTo-com.aspose.tasks.GenericProperty-TKey--}
```
public void CloneTo(GenericProperty<TKey> that)
```


Gör en djup kopia av instansen till en annan instans.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| that | [GenericProperty](../../com.aspose.tasks/genericproperty) | annan instans. |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### getName() {#getName--}
```
public final String getName()
```


Hämtar ett namn på egenskapen.

**Returns:**
java.lang.String - ett namn på egenskapen.
### getValue() {#getValue--}
```
public final Object getValue()
```


Hämtar ett värde på egenskapen.

**Returns:**
java.lang.Object - ett värde på egenskapen.
