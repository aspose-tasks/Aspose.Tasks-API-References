---
title: "Wert"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt einen Wert in einer Wertliste dar."
type: docs
weight: 333
url: /de/java/com.aspose.tasks/value/
---

**Inheritance:**
java.lang.Object
```
public class Value
```

Stellt einen Wert in einer Wertliste dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Value()](#Value--) | Initialisiert eine neue Instanz der [Value](../../com.aspose/tasks/value)-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getDateValue()](#getDateValue--) | Ruft den tatsächlichen Wert ab, wenn er als DateTime dargestellt werden kann. |
| [getDescription()](#getDescription--) | Ruft die Beschreibung eines Wertes ab. |
| [getDuration()](#getDuration--) | Ruft den tatsächlichen Wert ab, der zur Darstellung von Duration verwendet wird. |
| [getId()](#getId--) | Ruft die eindeutige Kennung eines Wertes projektübergreifend ab. |
| [getNumericValue()](#getNumericValue--) | Ruft den tatsächlichen Wert ab, der zur Darstellung von Zahlen- oder Kostenwerten verwendet wird. |
| [getPhonetic()](#getPhonetic--) | Ruft die phonetischen Informationen zum Namen des benutzerdefinierten Feldes ab. |
| [getStringValue()](#getStringValue--) | Ruft den tatsächlichen Wert ab, der zur Darstellung einer Textzeichenfolge verwendet wird. |
| [getVal()](#getVal--) | Ruft den tatsächlichen Wert in interner Darstellung ab. |
| [getValueGuid()](#getValueGuid--) | Ruft eine GUID ab, die diesen Wert im gesamten Projekt unter anderen identifiziert. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | Setzt den tatsächlichen Wert, wenn er als DateTime dargestellt werden kann. |
| [setDescription(String value)](#setDescription-java.lang.String-) | Setzt die Beschreibung eines Wertes. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Setzt den tatsächlichen Wert, der zur Darstellung von Duration verwendet wird. |
| [setId(int value)](#setId-int-) | Setzt die eindeutige Kennung eines Wertes projektübergreifend. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | Setzt den tatsächlichen Wert, der zur Darstellung von Zahlen- oder Kostenwerten verwendet wird. |
| [setPhonetic(String value)](#setPhonetic-java.lang.String-) | Setzt die phonetischen Informationen zum Namen des benutzerdefinierten Feldes. |
| [setStringValue(String value)](#setStringValue-java.lang.String-) | Setzt den tatsächlichen Wert, der zur Darstellung einer Textzeichenfolge verwendet wird. |
| [setVal(String value)](#setVal-java.lang.String-) | Setzt den tatsächlichen Wert in interner Darstellung. |
### Value() {#Value--}
```
public Value()
```


Initialisiert eine neue Instanz der [Value](../../com.aspose/tasks/value)-Klasse.

### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


Ruft den tatsächlichen Wert ab, wenn er als DateTime dargestellt werden kann. Der Standardwert ist DateTime\#MinValue.MinValue.

--------------------

Verwenden Sie diese Eigenschaft anstelle von `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), wenn Sie den DateTime‑Wert festlegen müssen.

**Returns:**
java.util.Date - der tatsächliche Wert, falls er als DateTime dargestellt werden kann.
### getDescription() {#getDescription--}
```
public final String getDescription()
```


Ruft die Beschreibung eines Wertes ab.

**Returns:**
java.lang.String - die Beschreibung eines Wertes.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Ruft den tatsächlichen Wert ab, der zur Darstellung von Duration verwendet wird.

--------------------

Verwenden Sie diese Eigenschaft anstelle von `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), wenn Sie den Duration‑Wert festlegen müssen.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the actual value which is used to represent Duration.
### getId() {#getId--}
```
public final int getId()
```


Ruft die eindeutige Kennung eines Wertes projektübergreifend ab.

Es ist wichtig, für verschiedene [Value](../../com.aspose.tasks/value)-Instanzen keine gleichen Bezeichner zu verwenden.

Der minimale `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-))-Wert ist `1`.

**Returns:**
int - der eindeutige Bezeichner eines Wertes im gesamten Projekt.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


Ruft den tatsächlichen Wert ab, der zur Darstellung von Zahlen- oder Kostenwerten verwendet wird.

--------------------

Verwenden Sie diese Eigenschaft anstelle von `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), wenn Sie den Number‑ oder Cost‑Wert festlegen müssen.

**Returns:**
java.math.BigDecimal - der tatsächliche Wert, der zur Darstellung von Zahlen‑ oder Kostenwerten verwendet wird.
### getPhonetic() {#getPhonetic--}
```
public final String getPhonetic()
```


Ruft die phonetischen Informationen zum Namen des benutzerdefinierten Feldes ab.

**Returns:**
java.lang.String - die phonetischen Informationen zum Namen des benutzerdefinierten Feldes.
### getStringValue() {#getStringValue--}
```
public final String getStringValue()
```


Ruft den tatsächlichen Wert ab, der zur Darstellung einer Textzeichenfolge verwendet wird.

--------------------

Verwenden Sie diese Eigenschaft anstelle von `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), wenn Sie den Textwert festlegen müssen.

**Returns:**
java.lang.String - der tatsächliche Wert, der zur Darstellung einer Textzeichenfolge verwendet wird.
### getVal() {#getVal--}
```
public final String getVal()
```


Gibt den tatsächlichen Wert in interner Darstellung zurück. Verwenden Sie vorzugsweise die unten aufgeführten stark typisierten Eigenschaften.

--------------------

Wenn Sie den Textwert festlegen möchten, verwenden Sie vorzugsweise die stark typisierte `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)) Eigenschaft.

Wenn Sie den Number‑ oder Cost‑Wert festlegen möchten, verwenden Sie vorzugsweise die stark typisierte `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)) Eigenschaft.

Wenn Sie Date/Start/Finish‑Werte festlegen möchten, verwenden Sie vorzugsweise die stark typisierte `DateValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)) Eigenschaft.

Wenn Sie den Duration‑Wert festlegen möchten, verwenden Sie vorzugsweise die stark typisierte `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)) Eigenschaft.

Falls Ihr Typ nicht aufgeführt ist, verwenden Sie die `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) Eigenschaft.

**Returns:**
java.lang.String - der tatsächliche Wert in interner Darstellung.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


Ruft eine GUID ab, die diesen Wert im gesamten Projekt unter anderen identifiziert.

**Returns:**
java.util.UUID - ein GUID, das diesen Wert im gesamten Projekt eindeutig identifiziert.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


Setzt den tatsächlichen Wert, falls er als DateTime dargestellt werden kann. Der Standardwert ist DateTime\#MinValue.MinValue.

--------------------

Verwenden Sie diese Eigenschaft anstelle von `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), wenn Sie den DateTime‑Wert festlegen müssen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | der tatsächliche Wert, falls er als DateTime dargestellt werden kann. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


Setzt die Beschreibung eines Wertes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | die Beschreibung eines Werts. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Setzt den tatsächlichen Wert, der zur Darstellung von Duration verwendet wird.

--------------------

Verwenden Sie diese Eigenschaft anstelle von `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), wenn Sie den Duration‑Wert festlegen müssen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | der tatsächliche Wert, der verwendet wird, um die Dauer darzustellen. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Setzt die eindeutige Kennung eines Wertes projektübergreifend.

Es ist wichtig, für verschiedene [Value](../../com.aspose.tasks/value)-Instanzen keine gleichen Bezeichner zu verwenden.

Der minimale `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-))-Wert ist `1`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | die eindeutige Kennung eines Werts über ein Projekt hinweg. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


Setzt den tatsächlichen Wert, der zur Darstellung von Zahlen- oder Kostenwerten verwendet wird.

--------------------

Verwenden Sie diese Eigenschaft anstelle von `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), wenn Sie den Number‑ oder Cost‑Wert festlegen müssen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.math.BigDecimal | der tatsächliche Wert, der verwendet wird, um eine Zahlen- oder Kostenangabe darzustellen. |

### setPhonetic(String value) {#setPhonetic-java.lang.String-}
```
public final void setPhonetic(String value)
```


Setzt die phonetischen Informationen zum Namen des benutzerdefinierten Feldes.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | die phonetischen Informationen zum Namen des benutzerdefinierten Feldes. |

### setStringValue(String value) {#setStringValue-java.lang.String-}
```
public final void setStringValue(String value)
```


Setzt den tatsächlichen Wert, der zur Darstellung einer Textzeichenfolge verwendet wird.

--------------------

Verwenden Sie diese Eigenschaft anstelle von `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), wenn Sie den Textwert festlegen müssen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | der tatsächliche Wert, der verwendet wird, um eine Textzeichenfolge darzustellen. |

### setVal(String value) {#setVal-java.lang.String-}
```
public final void setVal(String value)
```


Setzt den tatsächlichen Wert in der internen Darstellung. Verwenden Sie vorzugsweise stark typisierte Eigenschaften, die unten aufgeführt sind.

--------------------

Wenn Sie den Textwert festlegen möchten, verwenden Sie vorzugsweise die stark typisierte `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)) Eigenschaft.

Wenn Sie den Number‑ oder Cost‑Wert festlegen möchten, verwenden Sie vorzugsweise die stark typisierte `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)) Eigenschaft.

Wenn Sie Datums-/Start-/Endwerte festlegen möchten, verwenden Sie vorzugsweise die stark typisierte `DateTimeValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)) Eigenschaft.

Wenn Sie den Duration‑Wert festlegen möchten, verwenden Sie vorzugsweise die stark typisierte `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)) Eigenschaft.

Falls Ihr Typ nicht aufgeführt ist, verwenden Sie die `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) Eigenschaft.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | der tatsächliche Wert in der internen Darstellung. |

