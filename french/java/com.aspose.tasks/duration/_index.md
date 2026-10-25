---
title: "Duration"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente la durée dans un projet."
type: docs
weight: 76
url: /fr/java/com.aspose.tasks/duration/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public class Duration extends Struct<Duration> implements System.IEquatable<Duration>
```

Représente la durée dans un projet.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Duration()](#Duration--) | Initialise une nouvelle instance de la structure [Duration](../../com.aspose.tasks/duration) avec une valeur TimeSpan spécifiée et un TimeUnitType. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [Clone()](#Clone--) | Crée et renvoie une copie profonde de cette instance. |
| [CloneTo(Duration that)](#CloneTo-com.aspose.tasks.Duration-) | Effectue une copie profonde de l'instance dans une autre instance. |
| [add(Duration d)](#add-com.aspose.tasks.Duration-) | Ajoute la durée spécifiée à cette durée. |
| [add(double val)](#add-double-) | Ajoute la valeur double spécifiée à cette durée. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [convert(byte timeUnitType)](#convert-byte-) | Convertit l'objet Duration en une autre durée avec les unités de temps spécifiées. |
| [equals(Duration other)](#equals-com.aspose.tasks.Duration-) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [equals(Duration obj1, Duration obj2)](#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Renvoie une valeur indiquant si l'instance `obj1` spécifiée est égale à l'instance `obj2` spécifiée. |
| [equals(Object obj)](#equals-java.lang.Object-) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [getTimeSpan()](#getTimeSpan--) | Obtient l'instance `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\\#setTimeSpan-TimeSpan-)) de cet objet Duration. |
| [getTimeUnit()](#getTimeUnit--) | Obtient le type d'unité de temps pour cet objet. |
| [hashCode()](#hashCode--) | Renvoie une valeur de code de hachage pour cet objet. |
| [isElapsed()](#isElapsed--) | Obtient une valeur indiquant si l'unité de temps est écoulée. |
| [isEstimated()](#isEstimated--) | Obtient une valeur indiquant si l'unité de temps est estimée. |
| [op_Equality(Duration a, Duration b)](#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [op_Inequality(Duration a, Duration b)](#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Renvoie une valeur indiquant si cette instance n'est pas égale à un objet spécifié. |
| [parse(Project p, String value)](#parse-com.aspose.tasks.Project-java.lang.String-) | Convertit la chaîne spécifiée en instance de la structure [Duration](../../com.aspose/tasks/duration). |
| [parseTimeSpan(String value)](#parseTimeSpan-java.lang.String-) | Analyse la chaîne de durée au format "PT--H--M--S--". |
| [subtract(Duration d)](#subtract-com.aspose.tasks.Duration-) | Soustrait la durée spécifiée de cette instance de durée. |
| [subtract(double val)](#subtract-double-) | Soustrait la valeur double spécifiée de cette instance de durée. |
| [toDouble()](#toDouble--) | Convertit l'objet Duration en valeur `double`. |
| [toString()](#toString--) | Renvoie une représentation sous forme de chaîne de cette instance. |
### Duration() {#Duration--}
```
public Duration()
```


Initialise une nouvelle instance de la structure [Duration](../../com.aspose.tasks/duration) avec une valeur TimeSpan spécifiée et un TimeUnitType.

### Clone() {#Clone--}
```
public Duration Clone()
```


Crée et renvoie une copie profonde de cette instance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a deep copy of this object.
### CloneTo(Duration that) {#CloneTo-com.aspose.tasks.Duration-}
```
public void CloneTo(Duration that)
```


Effectue une copie profonde de l'instance dans une autre instance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| that | [Duration](../../com.aspose.tasks/duration) | une autre instance. |

### add(Duration d) {#add-com.aspose.tasks.Duration-}
```
public final Duration add(Duration d)
```


Ajoute la durée spécifiée à cette durée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | [Duration](../../com.aspose/tasks/duration) spécifié à ajouter à cette instance. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### add(double val) {#add-double-}
```
public final Duration add(double val)
```


Ajoute la valeur double spécifiée à cette durée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| val | double | la valeur `double` spécifiée à ajouter à cette instance. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### convert(byte timeUnitType) {#convert-byte-}
```
public final Duration convert(byte timeUnitType)
```


Convertit l'objet Duration en une autre durée avec les unités de temps spécifiées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| timeUnitType | byte | le type d'unité de temps spécifié. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - returns new duration with the specified unit type.
### equals(Duration other) {#equals-com.aspose.tasks.Duration-}
```
public final boolean equals(Duration other)
```


Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| other | [Duration](../../com.aspose.tasks/duration) | L'objet à comparer avec cette instance. |

**Returns:**
booléen - Renvoie **True** si une autre instance de Duration possède les mêmes valeurs TimeSpan et TimeUnit que cette instance; sinon, **false**.
### equals(Duration obj1, Duration obj2) {#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean equals(Duration obj1, Duration obj2)
```


Renvoie une valeur indiquant si l'instance `obj1` spécifiée est égale à l'instance `obj2` spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj1 | [Duration](../../com.aspose.tasks/duration) | le premier objet à comparer. |
| obj2 | [Duration](../../com.aspose.tasks/duration) | le deuxième objet à comparer. |

**Returns:**
boolean - renvoie true si l'instance `obj1` spécifiée est égale à l'instance `obj2` spécifiée ; sinon, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | L'objet à comparer avec cette instance. |

**Returns:**
booléen - **True** si l'objet spécifié est un Duration qui possède les mêmes valeurs TimeSpan et TimeUnit que cette instance; sinon, **false**.
### getTimeSpan() {#getTimeSpan--}
```
public final double getTimeSpan()
```


Obtient l'instance `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\\#setTimeSpan-TimeSpan-)) de cet objet Duration.

Valeur: L'instance TimeSpan de cet objet Duration.

**Returns:**
double - instance `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) de cet objet Duration.
### getTimeUnit() {#getTimeUnit--}
```
public final byte getTimeUnit()
```


Obtient le type d'unité de temps pour cet objet.

Valeur: Le type d'unité de temps de cette instance Duration.

**Returns:**
byte - type d'unité de temps pour cet objet.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Renvoie une valeur de code de hachage pour cet objet.

**Returns:**
int - renvoie une valeur de code de hachage pour cette instance de durée.
### isElapsed() {#isElapsed--}
```
public final boolean isElapsed()
```


Obtient une valeur indiquant si l'unité de temps est écoulée.

Valeur: Le drapeau qui détermine si cette instance Duration est écoulée.

**Returns:**
booléen - une valeur indiquant si l'unité de temps est écoulée.
### isEstimated() {#isEstimated--}
```
public final boolean isEstimated()
```


Obtient une valeur indiquant si l'unité de temps est estimée.

Valeur: Le drapeau qui détermine si cette instance Duration est estimée.

**Returns:**
booléen - une valeur indiquant si l'unité de temps est estimée.
### op_Equality(Duration a, Duration b) {#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Equality(Duration a, Duration b)
```


Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | La première durée. |
| b | [Duration](../../com.aspose.tasks/duration) | La deuxième durée. |

**Returns:**
booléen - une valeur indiquant si cette instance est égale à un objet spécifié
### op_Inequality(Duration a, Duration b) {#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Inequality(Duration a, Duration b)
```


Renvoie une valeur indiquant si cette instance n'est pas égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | La première durée. |
| b | [Duration](../../com.aspose.tasks/duration) | La deuxième durée. |

**Returns:**
booléen - une valeur indiquant si cette instance n'est pas égale à un objet spécifié
### parse(Project p, String value) {#parse-com.aspose.tasks.Project-java.lang.String-}
```
public static Duration parse(Project p, String value)
```


Convertit la chaîne spécifiée en instance de la structure [Duration](../../com.aspose/tasks/duration).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| p | [Project](../../com.aspose.tasks/project) | l'instance spécifiée de la classe [Project](../../com.aspose.tasks/project) pour convertir la durée. |
| valeur | java.lang.String | la chaîne spécifiée à convertir. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Returns the converted instance of [Duration](../../com.aspose.tasks/duration) struct.
### parseTimeSpan(String value) {#parseTimeSpan-java.lang.String-}
```
public static double parseTimeSpan(String value)
```


Analyse la chaîne de durée au format "PT--H--M--S--".

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | la chaîne spécifiée à analyser. |

**Returns:**
double - renvoie l'instance analysée de la structure `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)).
### subtract(Duration d) {#subtract-com.aspose.tasks.Duration-}
```
public final Duration subtract(Duration d)
```


Soustrait la durée spécifiée de cette instance de durée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | l'instance [Duration](../../com.aspose.tasks/duration) spécifiée à soustraire de cette instance. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### subtract(double val) {#subtract-double-}
```
public final Duration subtract(double val)
```


Soustrait la valeur double spécifiée de cette instance de durée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| val | double | valeur `double` spécifiée à soustraire de cette instance. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### toDouble() {#toDouble--}
```
public final double toDouble()
```


Convertit l'objet Duration en valeur `double`.

**Returns:**
double - Valeur convertie.
### toString() {#toString--}
```
public String toString()
```


Renvoie une représentation sous forme de chaîne de cette instance.

**Returns:**
java.lang.String - une représentation sous forme de chaîne de cette instance.
