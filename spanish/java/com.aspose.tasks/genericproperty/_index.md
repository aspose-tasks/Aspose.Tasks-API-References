---
title: "GenericProperty"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una propiedad de contenedor."
type: docs
weight: 113
url: /es/java/com.aspose.tasks/genericproperty/
---

**Inheritance:**
java.lang.Object
```
public class GenericProperty<TKey>
```

Representa una propiedad de contenedor.

TKey : El tipo de valor de la propiedad.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [GenericProperty()](#GenericProperty--) | Inicializa una nueva instancia de la clase GenericProperty&lt;T&gt;. |
| [GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name)](#GenericProperty-java.lang.Class-TKey--java.lang.String-) | Inicializa una nueva instancia de la estructura GenericProperty&lt;TKey&gt;. |
## Métodos

| Método | Descripción |
| --- | --- |
| [&lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2)](#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--) | Devuelve un valor que indica si la instancia `obj1` especificada es igual a la instancia `obj2` especificada. |
| [Clone()](#Clone--) | Crea y devuelve una copia profunda de esta instancia. |
| [CloneTo(GenericProperty&lt;TKey&gt; that)](#CloneTo-com.aspose.tasks.GenericProperty-TKey--) | Realiza una copia profunda de la instancia en otra instancia. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [equals(Object obj)](#equals-java.lang.Object-) | \{@inheritDoc\} |
| [getName()](#getName--) | Obtiene el nombre de la propiedad. |
| [getValue()](#getValue--) | Obtiene el valor de la propiedad. |
### GenericProperty() {#GenericProperty--}
```
public GenericProperty()
```


Inicializa una nueva instancia de la clase GenericProperty&lt;T&gt;.

### GenericProperty(Class&lt;TKey&gt; typeOfTKey, String name) {#GenericProperty-java.lang.Class-TKey--java.lang.String-}
```
public GenericProperty(Class<TKey> typeOfTKey, String name)
```


Inicializa una nueva instancia de la estructura GenericProperty&lt;TKey&gt;.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| typeOfTKey | java.lang.Class&lt;TKey&gt; |  |
| name | java.lang.String | El nombre de la propiedad. |

### &lt;TKey&gt;equals(GenericProperty&lt;TKey&gt; obj1, GenericProperty&lt;TKey&gt; obj2) {#-TKey-equals-com.aspose.tasks.GenericProperty-TKey--com.aspose.tasks.GenericProperty-TKey--}
```
public static boolean <TKey>equals(GenericProperty<TKey> obj1, GenericProperty<TKey> obj2)
```


Devuelve un valor que indica si la instancia `obj1` especificada es igual a la instancia `obj2` especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj1 | [GenericProperty](../../com.aspose.tasks/genericproperty) | el primer objeto a comparar. |
| obj2 | [GenericProperty](../../com.aspose.tasks/genericproperty) | el segundo objeto a comparar. |

**Returns:**
boolean - devuelve true si la instancia especificada `obj1` es igual a la instancia especificada `obj2`; de lo contrario, false.
### Clone() {#Clone--}
```
public GenericProperty<TKey> Clone()
```


Crea y devuelve una copia profunda de esta instancia.

**Returns:**
[GenericProperty](../../com.aspose.tasks/genericproperty) - a deep copy of this object.
### CloneTo(GenericProperty&lt;TKey&gt; that) {#CloneTo-com.aspose.tasks.GenericProperty-TKey--}
```
public void CloneTo(GenericProperty<TKey> that)
```


Realiza una copia profunda de la instancia en otra instancia.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| that | [GenericProperty](../../com.aspose.tasks/genericproperty) | otra instancia. |

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### getName() {#getName--}
```
public final String getName()
```


Obtiene el nombre de la propiedad.

**Returns:**
java.lang.String - un nombre de la propiedad.
### getValue() {#getValue--}
```
public final Object getValue()
```


Obtiene el valor de la propiedad.

**Returns:**
java.lang.Object - un valor de la propiedad.
