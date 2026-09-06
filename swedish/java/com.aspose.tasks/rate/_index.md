---
title: "Sats"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en definition av en tidsperiod och satser som gäller för en resurs under den perioden."
type: docs
weight: 232
url: /sv/java/com.aspose.tasks/rate/
---

**Inheritance:**
java.lang.Object
```
public class Rate
```

Representerar en definition av en tidsperiod och satser som gäller för en resurs under den perioden.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getCostPerUse()](#getCostPerUse--) | Hämtar kostnaden per användning av en resurs. |
| [getOvertimeRate()](#getOvertimeRate--) | Hämtar övertidssatsen per timme för en resurs. |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | Hämtar enheterna som Microsoft Project använder för att visa övertidssatsen. |
| [getRateTable()](#getRateTable--) | Hämtar den unika identifieraren för en taxatabell för en resurs. |
| [getRatesFrom()](#getRatesFrom--) | Hämtar datumet då en taxa blir gällande. |
| [getRatesTo()](#getRatesTo--) | Hämtar det sista datumet då en taxa är gällande. |
| [getStandardRate()](#getStandardRate--) | Hämtar standardtaxan per timme för en resurs. |
| [getStandardRateFormat()](#getStandardRateFormat--) | Hämtar enheterna som Microsoft Project använder för att visa standardtaxan. |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | Ställer in kostnaden per användning av en resurs. |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | Ställer in övertidssatsen per timme för en resurs. |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | Ställer in enheterna som Microsoft Project använder för att visa övertidssatsen. |
| [setRateTable(int value)](#setRateTable-int-) | Ställer in den unika identifieraren för en taxatabell för en resurs. |
| [setRatesFrom(Date value)](#setRatesFrom-java.util.Date-) | Ställer in datumet då en taxa blir gällande. |
| [setRatesTo(Date value)](#setRatesTo-java.util.Date-) | Ställer in det sista datumet då en taxa är gällande. |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | Ställer in standardtaxan per timme för en resurs. |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | Ställer in enheterna som Microsoft Project använder för att visa standardtaxan. |
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


Hämtar kostnaden per användning av en resurs. Detta värde hämtas från det aktuella datumet om en taxatabell finns för en resurs.

**Returns:**
java.math.BigDecimal - kostnaden per användning av en resurs.
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


Hämtar övertidssatsen per timme för en resurs.

**Returns:**
java.math.BigDecimal - övertidssatsen per timme för en resurs.
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


Hämtar enheterna som Microsoft Project använder för att visa övertidssatsen.

**Returns:**
int - enheterna som Microsoft Project använder för att visa övertidssatsen.
### getRateTable() {#getRateTable--}
```
public final int getRateTable()
```


Hämtar den unika identifieraren för en taxatabell för en resurs.

**Returns:**
int - den unika identifieraren för en taxatabell för en resurs.
### getRatesFrom() {#getRatesFrom--}
```
public final Date getRatesFrom()
```


Hämtar datumet då en taxa blir gällande.

**Returns:**
java.util.Date - datumet då en taxa blir gällande.
### getRatesTo() {#getRatesTo--}
```
public final Date getRatesTo()
```


Hämtar det sista datumet då en taxa är gällande.

**Returns:**
java.util.Date - det sista datumet då en taxa är gällande.
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


Hämtar standardtaxan per timme för en resurs.

**Returns:**
java.math.BigDecimal - standardtaxan per timme för en resurs.
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


Hämtar enheterna som Microsoft Project använder för att visa standardtaxan.

**Returns:**
int - enheterna som Microsoft Project använder för att visa standardtakten.
### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


Anger kostnaden per användning av en resurs. Detta värde hämtas från det aktuella datumet om en taxatabell finns för en resurs.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.math.BigDecimal | kostnaden per användning av en resurs. |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


Ställer in övertidssatsen per timme för en resurs.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.math.BigDecimal | övertidspriset per timme för en resurs. |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


Ställer in enheterna som Microsoft Project använder för att visa övertidssatsen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | enheterna som Microsoft Project använder för att visa övertidspriset. |

### setRateTable(int value) {#setRateTable-int-}
```
public final void setRateTable(int value)
```


Ställer in den unika identifieraren för en taxatabell för en resurs.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | den unika identifieraren för en taxatabell för en resurs. |

### setRatesFrom(Date value) {#setRatesFrom-java.util.Date-}
```
public final void setRatesFrom(Date value)
```


Ställer in datumet då en taxa blir gällande.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | datumet då ett pris blir giltigt. |

### setRatesTo(Date value) {#setRatesTo-java.util.Date-}
```
public final void setRatesTo(Date value)
```


Ställer in det sista datumet då en taxa är gällande.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | det sista datumet då ett pris är giltigt. |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


Ställer in standardtaxan per timme för en resurs.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.math.BigDecimal | standardpriset per timme för en resurs. |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


Ställer in enheterna som Microsoft Project använder för att visa standardtaxan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | enheterna som Microsoft Project använder för att visa standardpriset. |

