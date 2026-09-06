---
title: "Värde"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar ett värde i en värdelista."
type: docs
weight: 333
url: /sv/java/com.aspose.tasks/value/
---

**Inheritance:**
java.lang.Object
```
public class Value
```

Representerar ett värde i en värdelista.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Value()](#Value--) | Initierar en ny instans av klassen [Value](../../com.aspose/tasks/value). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getDateValue()](#getDateValue--) | Hämtar det faktiska värdet om det kan representeras som DateTime. |
| [getDescription()](#getDescription--) | Hämtar beskrivningen av ett värde. |
| [getDuration()](#getDuration--) | Hämtar det faktiska värdet som används för att representera varaktighet. |
| [getId()](#getId--) | Hämtar den unika identifieraren för ett värde i ett projekt. |
| [getNumericValue()](#getNumericValue--) | Hämtar det faktiska värdet som används för att representera tal- eller kostnadsvärde. |
| [getPhonetic()](#getPhonetic--) | Hämtar den fonetiska informationen om det anpassade fältets namn. |
| [getStringValue()](#getStringValue--) | Hämtar det faktiska värdet som används för att representera textsträng. |
| [getVal()](#getVal--) | Hämtar det faktiska värdet i intern representation. |
| [getValueGuid()](#getValueGuid--) | Hämtar en GUID som identifierar detta värde bland andra i hela projektet. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | Ställer in det faktiska värdet om det kan representeras som DateTime. |
| [setDescription(String value)](#setDescription-java.lang.String-) | Ställer in beskrivningen av ett värde. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Ställer in det faktiska värdet som används för att representera varaktighet. |
| [setId(int value)](#setId-int-) | Ställer in den unika identifieraren för ett värde i ett projekt. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | Ställer in det faktiska värdet som används för att representera tal- eller kostnadsvärde. |
| [setPhonetic(String value)](#setPhonetic-java.lang.String-) | Ställer in den fonetiska informationen om det anpassade fältets namn. |
| [setStringValue(String value)](#setStringValue-java.lang.String-) | Ställer in det faktiska värdet som används för att representera textsträng. |
| [setVal(String value)](#setVal-java.lang.String-) | Ställer in det faktiska värdet i intern representation. |
### Value() {#Value--}
```
public Value()
```


Initierar en ny instans av klassen [Value](../../com.aspose/tasks/value).

### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


Hämtar det faktiska värdet om det kan representeras som DateTime. Standardvärdet är DateTime\#MinValue.MinValue.

--------------------

Föredra den här egenskapen framför `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), när du behöver ange DateTime‑värdet.

**Returns:**
java.util.Date - det faktiska värdet om det kan representeras som DateTime.
### getDescription() {#getDescription--}
```
public final String getDescription()
```


Hämtar beskrivningen av ett värde.

**Returns:**
java.lang.String - beskrivningen av ett värde.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Hämtar det faktiska värdet som används för att representera varaktighet.

--------------------

Föredra den här egenskapen framför `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), när du behöver ange Duration‑värdet.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the actual value which is used to represent Duration.
### getId() {#getId--}
```
public final int getId()
```


Hämtar den unika identifieraren för ett värde i ett projekt.

Det är viktigt att inte ha samma identifierare för olika [Value](../../com.aspose.tasks/value)‑instanser.

Minimalt `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-))‑värde är `1`.

**Returns:**
int - det unika identifieraren för ett värde i hela projektet.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


Hämtar det faktiska värdet som används för att representera tal- eller kostnadsvärde.

--------------------

Föredra den här egenskapen framför `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), när du behöver ange Number‑ eller Cost‑värdet.

**Returns:**
java.math.BigDecimal - det faktiska värdet som används för att representera nummer‑ eller kostnadsvärde.
### getPhonetic() {#getPhonetic--}
```
public final String getPhonetic()
```


Hämtar den fonetiska informationen om det anpassade fältets namn.

**Returns:**
java.lang.String - den fonetiska informationen om det anpassade fältets namn.
### getStringValue() {#getStringValue--}
```
public final String getStringValue()
```


Hämtar det faktiska värdet som används för att representera textsträng.

--------------------

Föredra den här egenskapen framför `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), när du behöver ange Text‑värdet.

**Returns:**
java.lang.String - det faktiska värdet som används för att representera Text‑strängen.
### getVal() {#getVal--}
```
public final String getVal()
```


Hämtar det faktiska värdet i intern representation. Föredra att använda starkt typade egenskaper som listas nedan.

--------------------

Om du vill ange Text‑värde, föredra att använda starkt typad `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-))‑egenskap.

Om du vill ange Number‑ eller Cost‑värde, föredra att använda starkt typad `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-))‑egenskap.

Om du vill ange Date/Start/Finish‑värden, föredra att använda starkt typad `DateValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-))‑egenskap.

Om du vill ange Duration‑värde, föredra att använda starkt typad `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-))‑egenskap.

Om din typ inte finns med, använd `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-))‑egenskap.

**Returns:**
java.lang.String - det faktiska värdet i intern representation.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


Hämtar en GUID som identifierar detta värde bland andra i hela projektet.

**Returns:**
java.util.UUID - ett GUID som identifierar detta värde bland andra i hela projektet.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


Ställer in det faktiska värdet om det kan representeras som DateTime. Standardvärdet är DateTime\#MinValue.MinValue.

--------------------

Föredra den här egenskapen framför `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), när du behöver ange DateTime‑värdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | det faktiska värdet om det kan representeras som DateTime. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


Ställer in beskrivningen av ett värde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | beskrivningen av ett värde. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Ställer in det faktiska värdet som används för att representera varaktighet.

--------------------

Föredra den här egenskapen framför `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), när du behöver ange Duration‑värdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | det faktiska värdet som används för att representera Duration. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Ställer in den unika identifieraren för ett värde i ett projekt.

Det är viktigt att inte ha samma identifierare för olika [Value](../../com.aspose.tasks/value)‑instanser.

Minimalt `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-))‑värde är `1`.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | det unika identifieraren för ett värde över ett projekt. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


Ställer in det faktiska värdet som används för att representera tal- eller kostnadsvärde.

--------------------

Föredra den här egenskapen framför `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), när du behöver ange Number‑ eller Cost‑värdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.math.BigDecimal | det faktiska värdet som används för att representera nummer eller kostnadsvärde. |

### setPhonetic(String value) {#setPhonetic-java.lang.String-}
```
public final void setPhonetic(String value)
```


Ställer in den fonetiska informationen om det anpassade fältets namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | den fonetiska informationen om anpassat fältnamn. |

### setStringValue(String value) {#setStringValue-java.lang.String-}
```
public final void setStringValue(String value)
```


Ställer in det faktiska värdet som används för att representera textsträng.

--------------------

Föredra den här egenskapen framför `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), när du behöver ange Text‑värdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | det faktiska värdet som används för att representera textsträng. |

### setVal(String value) {#setVal-java.lang.String-}
```
public final void setVal(String value)
```


Ställer in det faktiska värdet i intern representation. Föredra att använda starkt typade egenskaper som listas nedan.

--------------------

Om du vill ange Text‑värde, föredra att använda starkt typad `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-))‑egenskap.

Om du vill ange Number‑ eller Cost‑värde, föredra att använda starkt typad `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-))‑egenskap.

Om du vill ange Date/Start/Finish‑värden, föredra att använda starkt typad `DateTimeValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)) egenskap.

Om du vill ange Duration‑värde, föredra att använda starkt typad `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-))‑egenskap.

Om din typ inte finns med, använd `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-))‑egenskap.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | det faktiska värdet i intern representation. |

