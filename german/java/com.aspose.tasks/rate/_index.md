---
title: "Rate"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Definition eines Zeitraums und der für eine Ressource in diesem Zeitraum geltenden Sätze dar."
type: docs
weight: 232
url: /de/java/com.aspose.tasks/rate/
---

**Inheritance:**
java.lang.Object
```
public class Rate
```

Stellt eine Definition eines Zeitraums und der für eine Ressource in diesem Zeitraum geltenden Sätze dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCostPerUse()](#getCostPerUse--) | Ermittelt die Kosten pro Nutzung einer Ressource. |
| [getOvertimeRate()](#getOvertimeRate--) | Ermittelt den Überstundensatz pro Stunde für eine Ressource. |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | Ermittelt die von Microsoft Project verwendeten Einheiten zur Anzeige des Überstundensatzes. |
| [getRateTable()](#getRateTable--) | Ermittelt die eindeutige Kennung einer Tariftabelle für eine Ressource. |
| [getRatesFrom()](#getRatesFrom--) | Ermittelt das Datum, an dem ein Tarif wirksam wird. |
| [getRatesTo()](#getRatesTo--) | Ermittelt das letzte Datum, an dem ein Tarif wirksam ist. |
| [getStandardRate()](#getStandardRate--) | Ermittelt den Standardtarif pro Stunde für eine Ressource. |
| [getStandardRateFormat()](#getStandardRateFormat--) | Ermittelt die von Microsoft Project verwendeten Einheiten zur Anzeige des Standardtarifs. |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | Legt die Kosten pro Nutzung einer Ressource fest. |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | Legt den Überstundensatz pro Stunde für eine Ressource fest. |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | Legt die von Microsoft Project verwendeten Einheiten zur Anzeige des Überstundensatzes fest. |
| [setRateTable(int value)](#setRateTable-int-) | Legt die eindeutige Kennung einer Tariftabelle für eine Ressource fest. |
| [setRatesFrom(Date value)](#setRatesFrom-java.util.Date-) | Legt das Datum fest, an dem ein Tarif wirksam wird. |
| [setRatesTo(Date value)](#setRatesTo-java.util.Date-) | Legt das letzte Datum fest, an dem ein Tarif wirksam ist. |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | Legt den Standardtarif pro Stunde für eine Ressource fest. |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | Legt die von Microsoft Project verwendeten Einheiten zur Anzeige des Standardtarifs fest. |
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


Ermittelt die Kosten pro Nutzung einer Ressource. Dieser Wert wird vom aktuellen Datum abgerufen, wenn für eine Ressource eine Tariftabelle existiert.

**Returns:**
java.math.BigDecimal - die Kosten pro Nutzung einer Ressource.
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


Ermittelt den Überstundensatz pro Stunde für eine Ressource.

**Returns:**
java.math.BigDecimal - der Überstundensatz pro Stunde für eine Ressource.
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


Ermittelt die von Microsoft Project verwendeten Einheiten zur Anzeige des Überstundensatzes.

**Returns:**
int - die Einheiten, die von Microsoft Project zur Anzeige des Überstundensatzes verwendet werden.
### getRateTable() {#getRateTable--}
```
public final int getRateTable()
```


Ermittelt die eindeutige Kennung einer Tariftabelle für eine Ressource.

**Returns:**
int - der eindeutige Bezeichner einer Tariftabelle für eine Ressource.
### getRatesFrom() {#getRatesFrom--}
```
public final Date getRatesFrom()
```


Ermittelt das Datum, an dem ein Tarif wirksam wird.

**Returns:**
java.util.Date - das Datum, an dem ein Tarif wirksam wird.
### getRatesTo() {#getRatesTo--}
```
public final Date getRatesTo()
```


Ermittelt das letzte Datum, an dem ein Tarif wirksam ist.

**Returns:**
java.util.Date - das letzte Datum, an dem ein Tarif wirksam ist.
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


Ermittelt den Standardtarif pro Stunde für eine Ressource.

**Returns:**
java.math.BigDecimal - der Standardsatz pro Stunde für eine Ressource.
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


Ermittelt die von Microsoft Project verwendeten Einheiten zur Anzeige des Standardtarifs.

**Returns:**
int - die Einheiten, die von Microsoft Project zur Anzeige des Standardsatzes verwendet werden.
### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


Legt die Kosten pro Nutzung einer Ressource fest. Dieser Wert wird vom aktuellen Datum abgerufen, wenn für eine Ressource eine Tariftabelle existiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.math.BigDecimal | die Kosten pro Nutzung einer Ressource. |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


Legt den Überstundensatz pro Stunde für eine Ressource fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.math.BigDecimal | der Überstundensatz pro Stunde für eine Ressource. |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


Legt die von Microsoft Project verwendeten Einheiten zur Anzeige des Überstundensatzes fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | die Einheiten, die von Microsoft Project zur Anzeige des Überstundensatzes verwendet werden. |

### setRateTable(int value) {#setRateTable-int-}
```
public final void setRateTable(int value)
```


Legt die eindeutige Kennung einer Tariftabelle für eine Ressource fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | der eindeutige Bezeichner einer Tariftabelle für eine Ressource. |

### setRatesFrom(Date value) {#setRatesFrom-java.util.Date-}
```
public final void setRatesFrom(Date value)
```


Legt das Datum fest, an dem ein Tarif wirksam wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | das Datum, an dem ein Tarif wirksam wird. |

### setRatesTo(Date value) {#setRatesTo-java.util.Date-}
```
public final void setRatesTo(Date value)
```


Legt das letzte Datum fest, an dem ein Tarif wirksam ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | das letzte Datum, an dem ein Tarif wirksam ist. |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


Legt den Standardtarif pro Stunde für eine Ressource fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.math.BigDecimal | der Standardsatz pro Stunde für eine Ressource. |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


Legt die von Microsoft Project verwendeten Einheiten zur Anzeige des Standardtarifs fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | die Einheiten, die von Microsoft Project zur Anzeige des Standardsatzes verwendet werden. |

