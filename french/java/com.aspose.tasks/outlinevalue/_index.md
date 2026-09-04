---
title: "OutlineValue"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une valeur de plan."
type: docs
weight: 173
url: /fr/java/com.aspose.tasks/outlinevalue/
---

**Inheritance:**
java.lang.Object
```
public class OutlineValue
```

Représente une valeur de plan.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [OutlineValue()](#OutlineValue--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getDescription()](#getDescription--) | Obtient la description d'une valeur de plan. |
| [getDurationValue()](#getDurationValue--) | Obtient la durée si le Type est Duration. |
| [getParentValueId()](#getParentValueId--) | Obtient l'Id d'un nœud parent d'un code de plan. |
| [getType()](#getType--) | Obtient le type de code de plan. |
| [getValue()](#getValue--) | Obtient la valeur réelle. |
| [getValueGuid()](#getValueGuid--) | Obtient un GUID qui identifie cette valeur parmi les autres dans l'ensemble du projet. |
| [getValueId()](#getValueId--) | Obtient l'Id unique d'une valeur de code de plan au sein d'un projet. |
| [isCollapsed()](#isCollapsed--) | Obtient une valeur indiquant si la valeur de plan est réduite ou non. |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | Définit une valeur indiquant si la valeur de plan est réduite ou non. |
| [setDescription(String value)](#setDescription-java.lang.String-) | Définit la description d'une valeur de plan. |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | Définit la durée si le Type est Duration. |
| [setParentValueId(int value)](#setParentValueId-int-) | Définit l'Id d'un nœud parent d'un code de plan. |
| [setType(int value)](#setType-int-) | Définit le type de code de plan. |
| [setValue(String value)](#setValue-java.lang.String-) | Définit la valeur réelle. |
| [setValueId(int value)](#setValueId-int-) | Définit l'Id unique d'une valeur de code de plan au sein d'un projet. |
### OutlineValue() {#OutlineValue--}
```
public OutlineValue()
```


### getDescription() {#getDescription--}
```
public final String getDescription()
```


Obtient la description d'une valeur de plan.

**Returns:**
java.lang.String - la description d'une valeur de plan.
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


Obtient la durée si le Type est Duration.

--------------------

Préférez cette propriété plutôt que le `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)), lorsque vous devez définir la valeur pour les OutlineValues de type Duration.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration if Type is Duration.
### getParentValueId() {#getParentValueId--}
```
public final int getParentValueId()
```


Obtient l'Id d'un nœud parent d'un code de plan.

**Returns:**
int - l'Id d'un nœud parent d'un code de plan.
### getType() {#getType--}
```
public final int getType()
```


Obtient le type de code de plan.

**Returns:**
int - le type de code de plan.
### getValue() {#getValue--}
```
public final String getValue()
```


Obtient la valeur réelle.

**Returns:**
java.lang.String - la valeur réelle.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


Obtient un GUID qui identifie cette valeur parmi les autres dans l'ensemble du projet.

**Returns:**
java.util.UUID - un GUID qui identifie cette valeur parmi les autres dans l'ensemble du projet.
### getValueId() {#getValueId--}
```
public final int getValueId()
```


Obtient l'Id unique d'une valeur de code de plan au sein d'un projet.

**Returns:**
int - l'Id unique d'une valeur de code de plan au sein d'un projet.
### isCollapsed() {#isCollapsed--}
```
public final boolean isCollapsed()
```


Obtient une valeur indiquant si la valeur de plan est réduite ou non.

--------------------

Ceci est une nouvelle propriété pour MS Project 2010.

**Returns:**
boolean - une valeur indiquant si la valeur de plan est réduite ou non.
### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public final void setCollapsed(boolean value)
```


Définit une valeur indiquant si la valeur de plan est réduite ou non.

--------------------

Ceci est une nouvelle propriété pour MS Project 2010.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si la valeur de plan est réduite ou non. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


Définit la description d'une valeur de plan.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | la description d'une valeur de plan. |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


Définit la durée si le Type est Duration.

--------------------

Préférez cette propriété plutôt que le `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)), lorsque vous devez définir la valeur pour les OutlineValues de type Duration.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | la durée si le type est Durée. |

### setParentValueId(int value) {#setParentValueId-int-}
```
public final void setParentValueId(int value)
```


Définit l'Id d'un nœud parent d'un code de plan.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | l'ID d'un nœud parent d'un code de plan. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Définit le type de code de plan.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | le type de code de plan. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


Définit la valeur réelle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | la valeur réelle. |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


Définit l'Id unique d'une valeur de code de plan au sein d'un projet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | l'ID unique d'une valeur de code de plan dans un projet. |

