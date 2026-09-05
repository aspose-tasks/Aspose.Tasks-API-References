---
title: "Waarde"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een waarde in een waardelijst voor."
type: docs
weight: 333
url: /nl/java/com.aspose.tasks/value/
---

**Inheritance:**
java.lang.Object
```
public class Value
```

Stelt een waarde in een waardelijst voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Value()](#Value--) | Initialiseert een nieuw exemplaar van de klasse [Value](../../com.aspose.tasks/value). |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getDateValue()](#getDateValue--) | Haalt de werkelijke waarde op als deze kan worden weergegeven als DateTime. |
| [getDescription()](#getDescription--) | Haalt de beschrijving van een waarde op. |
| [getDuration()](#getDuration--) | Haalt de werkelijke waarde op die wordt gebruikt om Duur weer te geven. |
| [getId()](#getId--) | Haalt de unieke identifier van een waarde op binnen een project. |
| [getNumericValue()](#getNumericValue--) | Haalt de werkelijke waarde op die wordt gebruikt om een getal of kostwaarde weer te geven. |
| [getPhonetic()](#getPhonetic--) | Haalt de fonetische informatie over de naam van het aangepaste veld op. |
| [getStringValue()](#getStringValue--) | Haalt de werkelijke waarde op die wordt gebruikt om een tekstreeks weer te geven. |
| [getVal()](#getVal--) | Haalt de werkelijke waarde op in interne representatie. |
| [getValueGuid()](#getValueGuid--) | Haalt een GUID op die deze waarde identificeert tussen andere in het gehele project. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | Stelt de werkelijke waarde in als deze kan worden weergegeven als DateTime. |
| [setDescription(String value)](#setDescription-java.lang.String-) | Stelt de beschrijving van een waarde in. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Stelt de werkelijke waarde in die wordt gebruikt om Duur weer te geven. |
| [setId(int value)](#setId-int-) | Stelt de unieke identifier van een waarde in binnen een project. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | Stelt de werkelijke waarde in die wordt gebruikt om een getal of kostwaarde weer te geven. |
| [setPhonetic(String value)](#setPhonetic-java.lang.String-) | Stelt de fonetische informatie over de naam van het aangepaste veld in. |
| [setStringValue(String value)](#setStringValue-java.lang.String-) | Stelt de werkelijke waarde in die wordt gebruikt om een tekstreeks weer te geven. |
| [setVal(String value)](#setVal-java.lang.String-) | Stelt de werkelijke waarde in in interne representatie. |
### Value() {#Value--}
```
public Value()
```


Initialiseert een nieuw exemplaar van de klasse [Value](../../com.aspose.tasks/value).

### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


Haalt de werkelijke waarde op als deze kan worden weergegeven als DateTime. Standaardwaarde is DateTime\#MinValue.MinValue.

--------------------

Geef de voorkeur aan deze eigenschap boven de `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)), wanneer u de DateTime‑waarde moet instellen.

**Returns:**
java.util.Date - de werkelijke waarde als deze kan worden weergegeven als DateTime.
### getDescription() {#getDescription--}
```
public final String getDescription()
```


Haalt de beschrijving van een waarde op.

**Returns:**
java.lang.String - de beschrijving van een waarde.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Haalt de werkelijke waarde op die wordt gebruikt om Duur weer te geven.

--------------------

Geef de voorkeur aan deze eigenschap boven de `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)), wanneer u de Duration‑waarde moet instellen.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the actual value which is used to represent Duration.
### getId() {#getId--}
```
public final int getId()
```


Haalt de unieke identifier van een waarde op binnen een project.

Het is belangrijk om niet dezelfde identifiers te hebben voor verschillende [Value](../../com.aspose/tasks/value) instanties.

De minimale `Id`([getId()](../../com.aspose/tasks/value\#getId--)/[setId(int)](../../com.aspose/tasks/value\#setId-int-)) waarde is `1`.

**Returns:**
int - de unieke identifier van een waarde binnen een project.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


Haalt de werkelijke waarde op die wordt gebruikt om een getal of kostwaarde weer te geven.

--------------------

Geef de voorkeur aan deze eigenschap boven de `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)), wanneer u de Number‑ of Cost‑waarde moet instellen.

**Returns:**
java.math.BigDecimal - de werkelijke waarde die wordt gebruikt om een nummer‑ of kostenwaarde weer te geven.
### getPhonetic() {#getPhonetic--}
```
public final String getPhonetic()
```


Haalt de fonetische informatie over de naam van het aangepaste veld op.

**Returns:**
java.lang.String - de fonetische informatie over de naam van het aangepaste veld.
### getStringValue() {#getStringValue--}
```
public final String getStringValue()
```


Haalt de werkelijke waarde op die wordt gebruikt om een tekstreeks weer te geven.

--------------------

Geef de voorkeur aan deze eigenschap boven de `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)), wanneer u de Text‑waarde moet instellen.

**Returns:**
java.lang.String - de werkelijke waarde die wordt gebruikt om een Text‑tekenreeks weer te geven.
### getVal() {#getVal--}
```
public final String getVal()
```


Haalt de werkelijke waarde op in de interne representatie. Geef de voorkeur aan het gebruik van sterk getypeerde eigenschappen die hieronder worden vermeld.

--------------------

Als u Text‑waarde wilt instellen, geef dan de voorkeur aan het gebruik van de sterk getypeerde `StringValue`([getStringValue()](../../com.aspose/tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose/tasks/value\#setStringValue-String-)) eigenschap.

Als u Number‑ of Cost‑waarde wilt instellen, geef dan de voorkeur aan het gebruik van de sterk getypeerde `NumericValue`([getNumericValue()](../../com.aspose/tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose/tasks/value\#setNumericValue-java.math.BigDecimal-)) eigenschap.

Als u Date/Start/Finish‑waarden wilt instellen, geef dan de voorkeur aan het gebruik van de sterk getypeerde `DateValue`([getDateValue()](../../com.aspose/tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose/tasks/value\#setDateValue-java.util.Date-)) eigenschap.

Als u Duration‑waarde wilt instellen, geef dan de voorkeur aan het gebruik van de sterk getypeerde `Duration`([getDuration()](../../com.aspose/tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose/tasks/value\#setDuration-Duration-)) eigenschap.

Als uw type niet is vermeld, gebruik dan de `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)) eigenschap.

**Returns:**
java.lang.String - de werkelijke waarde in interne representatie.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


Haalt een GUID op die deze waarde identificeert tussen andere in het gehele project.

**Returns:**
java.util.UUID - een GUID die deze waarde identificeert tussen andere waarden in het gehele project.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


Stelt de werkelijke waarde in als deze kan worden weergegeven als DateTime. Standaardwaarde is DateTime\#MinValue.MinValue.

--------------------

Geef de voorkeur aan deze eigenschap boven de `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)), wanneer u de DateTime‑waarde moet instellen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | de werkelijke waarde als deze kan worden weergegeven als DateTime. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


Stelt de beschrijving van een waarde in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de beschrijving van een waarde. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Stelt de werkelijke waarde in die wordt gebruikt om Duur weer te geven.

--------------------

Geef de voorkeur aan deze eigenschap boven de `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)), wanneer u de Duration‑waarde moet instellen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | de werkelijke waarde die wordt gebruikt om Duration weer te geven. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Stelt de unieke identifier van een waarde in binnen een project.

Het is belangrijk om niet dezelfde identifiers te hebben voor verschillende [Value](../../com.aspose/tasks/value) instanties.

De minimale `Id`([getId()](../../com.aspose/tasks/value\#getId--)/[setId(int)](../../com.aspose/tasks/value\#setId-int-)) waarde is `1`.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de unieke identifier van een waarde over een project. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


Stelt de werkelijke waarde in die wordt gebruikt om een getal of kostwaarde weer te geven.

--------------------

Geef de voorkeur aan deze eigenschap boven de `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)), wanneer u de Number‑ of Cost‑waarde moet instellen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.math.BigDecimal | de werkelijke waarde die wordt gebruikt om een getal of kostenwaarde weer te geven. |

### setPhonetic(String value) {#setPhonetic-java.lang.String-}
```
public final void setPhonetic(String value)
```


Stelt de fonetische informatie over de naam van het aangepaste veld in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de fonetische informatie over de naam van het aangepaste veld. |

### setStringValue(String value) {#setStringValue-java.lang.String-}
```
public final void setStringValue(String value)
```


Stelt de werkelijke waarde in die wordt gebruikt om een tekstreeks weer te geven.

--------------------

Geef de voorkeur aan deze eigenschap boven de `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)), wanneer u de Text‑waarde moet instellen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de werkelijke waarde die wordt gebruikt om een tekststring weer te geven. |

### setVal(String value) {#setVal-java.lang.String-}
```
public final void setVal(String value)
```


Stelt de werkelijke waarde in de interne representatie in. Gebruik bij voorkeur sterk getypeerde eigenschappen die hieronder worden vermeld.

--------------------

Als u Text‑waarde wilt instellen, geef dan de voorkeur aan het gebruik van de sterk getypeerde `StringValue`([getStringValue()](../../com.aspose/tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose/tasks/value\#setStringValue-String-)) eigenschap.

Als u Number‑ of Cost‑waarde wilt instellen, geef dan de voorkeur aan het gebruik van de sterk getypeerde `NumericValue`([getNumericValue()](../../com.aspose/tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose/tasks/value\#setNumericValue-java.math.BigDecimal-)) eigenschap.

Als je Date/Start/Finish-waarden wilt instellen, gebruik dan bij voorkeur de sterk getypeerde `DateTimeValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)) eigenschap.

Als u Duration‑waarde wilt instellen, geef dan de voorkeur aan het gebruik van de sterk getypeerde `Duration`([getDuration()](../../com.aspose/tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose/tasks/value\#setDuration-Duration-)) eigenschap.

Als uw type niet is vermeld, gebruik dan de `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)) eigenschap.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de werkelijke waarde in de interne representatie. |

