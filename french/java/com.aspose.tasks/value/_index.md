---
title: "Valeur"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une valeur dans une liste de valeurs."
type: docs
weight: 333
url: /fr/java/com.aspose.tasks/value/
---

**Inheritance:**
java.lang.Object
```
public class Value
```

Représente une valeur dans une liste de valeurs.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Value()](#Value--) | Initialise une nouvelle instance de la classe [Value](../../com.aspose/tasks/value). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getDateValue()](#getDateValue--) | Obtient la valeur réelle si elle peut être représentée en tant que DateTime. |
| [getDescription()](#getDescription--) | Obtient la description d'une valeur. |
| [getDuration()](#getDuration--) | Obtient la valeur réelle utilisée pour représenter la durée. |
| [getId()](#getId--) | Obtient l'identifiant unique d'une valeur à travers un projet. |
| [getNumericValue()](#getNumericValue--) | Obtient la valeur réelle utilisée pour représenter une valeur numérique ou de coût. |
| [getPhonetic()](#getPhonetic--) | Obtient les informations phonétiques concernant le nom du champ personnalisé. |
| [getStringValue()](#getStringValue--) | Obtient la valeur réelle utilisée pour représenter une chaîne de texte. |
| [getVal()](#getVal--) | Obtient la valeur réelle en représentation interne. |
| [getValueGuid()](#getValueGuid--) | Obtient un GUID qui identifie cette valeur parmi les autres dans l'ensemble du projet. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | Définit la valeur réelle si elle peut être représentée en tant que DateTime. |
| [setDescription(String value)](#setDescription-java.lang.String-) | Définit la description d'une valeur. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Définit la valeur réelle utilisée pour représenter la durée. |
| [setId(int value)](#setId-int-) | Définit l'identifiant unique d'une valeur à travers un projet. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | Définit la valeur réelle utilisée pour représenter une valeur numérique ou de coût. |
| [setPhonetic(String value)](#setPhonetic-java.lang.String-) | Définit les informations phonétiques concernant le nom du champ personnalisé. |
| [setStringValue(String value)](#setStringValue-java.lang.String-) | Définit la valeur réelle utilisée pour représenter une chaîne de texte. |
| [setVal(String value)](#setVal-java.lang.String-) | Définit la valeur réelle en représentation interne. |
### Value() {#Value--}
```
public Value()
```


Initialise une nouvelle instance de la classe [Value](../../com.aspose/tasks/value).

### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


Obtient la valeur réelle si elle peut être représentée en tant que DateTime. La valeur par défaut est DateTime\#MinValue.MinValue.

--------------------

Préférez cette propriété plutôt que le `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), lorsque vous devez définir la valeur DateTime.

**Returns:**
java.util.Date - la valeur réelle si elle peut être représentée comme DateTime.
### getDescription() {#getDescription--}
```
public final String getDescription()
```


Obtient la description d'une valeur.

**Returns:**
java.lang.String - la description d'une valeur.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Obtient la valeur réelle utilisée pour représenter la durée.

--------------------

Préférez cette propriété plutôt que le `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), lorsque vous devez définir la valeur Duration.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the actual value which is used to represent Duration.
### getId() {#getId--}
```
public final int getId()
```


Obtient l'identifiant unique d'une valeur à travers un projet.

Il est important de ne pas avoir les mêmes identifiants pour différentes instances de [Value](../../com.aspose.tasks/value).

La valeur minimale de `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-)) est `1`.

**Returns:**
int - l'identifiant unique d'une valeur dans l'ensemble d'un projet.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


Obtient la valeur réelle utilisée pour représenter une valeur numérique ou de coût.

--------------------

Préférez cette propriété plutôt que le `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), lorsque vous devez définir la valeur Number ou Cost.

**Returns:**
java.math.BigDecimal - la valeur réelle utilisée pour représenter la valeur nombre ou coût.
### getPhonetic() {#getPhonetic--}
```
public final String getPhonetic()
```


Obtient les informations phonétiques concernant le nom du champ personnalisé.

**Returns:**
java.lang.String - l'information phonétique concernant le nom du champ personnalisé.
### getStringValue() {#getStringValue--}
```
public final String getStringValue()
```


Obtient la valeur réelle utilisée pour représenter une chaîne de texte.

--------------------

Préférez cette propriété plutôt que le `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), lorsque vous devez définir la valeur Text.

**Returns:**
java.lang.String - la valeur réelle utilisée pour représenter la chaîne Text.
### getVal() {#getVal--}
```
public final String getVal()
```


Obtient la valeur réelle en représentation interne. Préférez utiliser les propriétés fortement typées listées ci-dessous.

--------------------

Si vous souhaitez définir une valeur Text, privilégiez l'utilisation de la propriété fortement typée `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)).

Si vous souhaitez définir une valeur Number ou Cost, privilégiez l'utilisation de la propriété fortement typée `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)).

Si vous souhaitez définir des valeurs Date/Start/Finish, privilégiez l'utilisation de la propriété fortement typée `DateValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)).

Si vous souhaitez définir une valeur Duration, privilégiez l'utilisation de la propriété fortement typée `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)).

Si votre type n'est pas répertorié, utilisez la propriété `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)).

**Returns:**
java.lang.String - la valeur réelle en représentation interne.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


Obtient un GUID qui identifie cette valeur parmi les autres dans l'ensemble du projet.

**Returns:**
java.util.UUID - un GUID qui identifie cette valeur parmi les autres dans l'ensemble du projet.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


Définit la valeur réelle si elle peut être représentée comme DateTime. La valeur par défaut est DateTime\#MinValue.MinValue.

--------------------

Préférez cette propriété plutôt que le `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), lorsque vous devez définir la valeur DateTime.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | la valeur réelle si elle peut être représentée comme DateTime. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


Définit la description d'une valeur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | la description d'une valeur. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Définit la valeur réelle utilisée pour représenter la durée.

--------------------

Préférez cette propriété plutôt que le `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), lorsque vous devez définir la valeur Duration.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | la valeur réelle utilisée pour représenter la Duration. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Définit l'identifiant unique d'une valeur à travers un projet.

Il est important de ne pas avoir les mêmes identifiants pour différentes instances de [Value](../../com.aspose.tasks/value).

La valeur minimale de `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-)) est `1`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | l'identifiant unique d'une valeur dans un projet. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


Définit la valeur réelle utilisée pour représenter une valeur numérique ou de coût.

--------------------

Préférez cette propriété plutôt que le `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), lorsque vous devez définir la valeur Number ou Cost.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.math.BigDecimal | la valeur réelle utilisée pour représenter un nombre ou une valeur de coût. |

### setPhonetic(String value) {#setPhonetic-java.lang.String-}
```
public final void setPhonetic(String value)
```


Définit les informations phonétiques concernant le nom du champ personnalisé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | les informations phonétiques concernant le nom du champ personnalisé. |

### setStringValue(String value) {#setStringValue-java.lang.String-}
```
public final void setStringValue(String value)
```


Définit la valeur réelle utilisée pour représenter une chaîne de texte.

--------------------

Préférez cette propriété plutôt que le `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), lorsque vous devez définir la valeur Text.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | la valeur réelle utilisée pour représenter une chaîne de texte. |

### setVal(String value) {#setVal-java.lang.String-}
```
public final void setVal(String value)
```


Définit la valeur réelle dans la représentation interne. Privilégiez l'utilisation de propriétés fortement typées listées ci-dessous.

--------------------

Si vous souhaitez définir une valeur Text, privilégiez l'utilisation de la propriété fortement typée `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)).

Si vous souhaitez définir une valeur Number ou Cost, privilégiez l'utilisation de la propriété fortement typée `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)).

Si vous voulez définir les valeurs Date/Début/Fin, privilégiez l'utilisation de la propriété fortement typée `DateTimeValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)).

Si vous souhaitez définir une valeur Duration, privilégiez l'utilisation de la propriété fortement typée `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)).

Si votre type n'est pas répertorié, utilisez la propriété `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | la valeur réelle dans la représentation interne. |

