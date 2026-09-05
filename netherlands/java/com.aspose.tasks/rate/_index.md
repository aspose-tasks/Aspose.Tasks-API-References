---
title: "Tarief"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een definitie van een tijdsperiode en tarieven die van toepassing zijn op een resource gedurende die periode voor."
type: docs
weight: 232
url: /nl/java/com.aspose.tasks/rate/
---

**Inheritance:**
java.lang.Object
```
public class Rate
```

Stelt een definitie van een tijdsperiode en tarieven die van toepassing zijn op een resource gedurende die periode voor.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getCostPerUse()](#getCostPerUse--) | Haalt de kosten per gebruik van een resource op. |
| [getOvertimeRate()](#getOvertimeRate--) | Haalt het overurenttarief per uur voor een resource op. |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | Haalt de eenheden op die Microsoft Project gebruikt om het overurenttarief weer te geven. |
| [getRateTable()](#getRateTable--) | Haalt de unieke identifier op van een tarieftabel voor een resource. |
| [getRatesFrom()](#getRatesFrom--) | Haalt de datum op waarop een tarief van kracht wordt. |
| [getRatesTo()](#getRatesTo--) | Haalt de laatste datum op waarop een tarief van kracht is. |
| [getStandardRate()](#getStandardRate--) | Haalt het standaardtarief per uur voor een resource op. |
| [getStandardRateFormat()](#getStandardRateFormat--) | Haalt de eenheden op die Microsoft Project gebruikt om het standaardtarief weer te geven. |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | Stelt de kosten per gebruik van een resource in. |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | Stelt het overurenttarief per uur voor een resource in. |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | Stelt de eenheden in die door Microsoft Project worden gebruikt om het overurenttarief weer te geven. |
| [setRateTable(int value)](#setRateTable-int-) | Stelt de unieke identifier van een tarieftabel voor een resource in. |
| [setRatesFrom(Date value)](#setRatesFrom-java.util.Date-) | Stelt de datum in waarop een tarief van kracht wordt. |
| [setRatesTo(Date value)](#setRatesTo-java.util.Date-) | Stelt de laatste datum in waarop een tarief van kracht is. |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | Stelt het standaardtarief per uur voor een resource in. |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | Stelt de eenheden in die door Microsoft Project worden gebruikt om het standaardtarief weer te geven. |
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


Haalt de kosten per gebruik van een resource op. Deze waarde wordt opgehaald op basis van de huidige datum als er een tarieftabel voor een resource bestaat.

**Returns:**
java.math.BigDecimal - de kosten per gebruik van een resource.
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


Haalt het overurenttarief per uur voor een resource op.

**Returns:**
java.math.BigDecimal - het overurenttarief per uur voor een resource.
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


Haalt de eenheden op die Microsoft Project gebruikt om het overurenttarief weer te geven.

**Returns:**
int - de eenheden die door Microsoft Project worden gebruikt om het overurenttarief weer te geven.
### getRateTable() {#getRateTable--}
```
public final int getRateTable()
```


Haalt de unieke identifier op van een tarieftabel voor een resource.

**Returns:**
int - de unieke identifier van een tarieftabel voor een resource.
### getRatesFrom() {#getRatesFrom--}
```
public final Date getRatesFrom()
```


Haalt de datum op waarop een tarief van kracht wordt.

**Returns:**
java.util.Date - de datum waarop een tarief van kracht wordt.
### getRatesTo() {#getRatesTo--}
```
public final Date getRatesTo()
```


Haalt de laatste datum op waarop een tarief van kracht is.

**Returns:**
java.util.Date - de laatste datum waarop een tarief van kracht is.
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


Haalt het standaardtarief per uur voor een resource op.

**Returns:**
java.math.BigDecimal - het standaardtarief per uur voor een resource.
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


Haalt de eenheden op die Microsoft Project gebruikt om het standaardtarief weer te geven.

**Returns:**
int - de eenheden die door Microsoft Project worden gebruikt om het standaardtarief weer te geven.
### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


Stelt de kosten per gebruik van een resource in. Deze waarde wordt opgehaald op basis van de huidige datum als er een tarieftabel voor een resource bestaat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.math.BigDecimal | de kosten per gebruik van een resource. |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


Stelt het overurenttarief per uur voor een resource in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.math.BigDecimal | het overurenttarief per uur voor een resource. |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


Stelt de eenheden in die door Microsoft Project worden gebruikt om het overurenttarief weer te geven.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de eenheden die door Microsoft Project worden gebruikt om het overurenttarief weer te geven. |

### setRateTable(int value) {#setRateTable-int-}
```
public final void setRateTable(int value)
```


Stelt de unieke identifier van een tarieftabel voor een resource in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de unieke identifier van een tarieftabel voor een resource. |

### setRatesFrom(Date value) {#setRatesFrom-java.util.Date-}
```
public final void setRatesFrom(Date value)
```


Stelt de datum in waarop een tarief van kracht wordt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | de datum waarop een tarief van kracht wordt. |

### setRatesTo(Date value) {#setRatesTo-java.util.Date-}
```
public final void setRatesTo(Date value)
```


Stelt de laatste datum in waarop een tarief van kracht is.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | de laatste datum waarop een tarief van kracht is. |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


Stelt het standaardtarief per uur voor een resource in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.math.BigDecimal | het standaardtarief per uur voor een resource. |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


Stelt de eenheden in die door Microsoft Project worden gebruikt om het standaardtarief weer te geven.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de eenheden die door Microsoft Project worden gebruikt om het standaardtarief weer te geven. |

