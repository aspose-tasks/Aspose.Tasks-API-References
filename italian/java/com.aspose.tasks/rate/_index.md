---
title: "Tariffa"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta una definizione di un periodo di tempo e delle tariffe applicabili a una risorsa durante tale periodo."
type: docs
weight: 232
url: /it/java/com.aspose.tasks/rate/
---

**Inheritance:**
java.lang.Object
```
public class Rate
```

Rappresenta una definizione di un periodo di tempo e delle tariffe applicabili a una risorsa durante tale periodo.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getCostPerUse()](#getCostPerUse--) | Ottiene il costo per utilizzo di una risorsa. |
| [getOvertimeRate()](#getOvertimeRate--) | Ottiene la tariffa degli straordinari per ora per una risorsa. |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | Ottiene le unità utilizzate da Microsoft Project per visualizzare la tariffa degli straordinari. |
| [getRateTable()](#getRateTable--) | Ottiene l'identificatore univoco di una tabella delle tariffe per una risorsa. |
| [getRatesFrom()](#getRatesFrom--) | Ottiene la data in cui una tariffa entra in vigore. |
| [getRatesTo()](#getRatesTo--) | Ottiene l'ultima data in cui una tariffa è valida. |
| [getStandardRate()](#getStandardRate--) | Ottiene la tariffa standard per ora per una risorsa. |
| [getStandardRateFormat()](#getStandardRateFormat--) | Ottiene le unità utilizzate da Microsoft Project per visualizzare la tariffa standard. |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | Imposta il costo per utilizzo di una risorsa. |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | Imposta la tariffa degli straordinari per ora per una risorsa. |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | Imposta le unità utilizzate da Microsoft Project per visualizzare la tariffa degli straordinari. |
| [setRateTable(int value)](#setRateTable-int-) | Imposta l'identificatore univoco di una tabella delle tariffe per una risorsa. |
| [setRatesFrom(Date value)](#setRatesFrom-java.util.Date-) | Imposta la data in cui una tariffa diventa effettiva. |
| [setRatesTo(Date value)](#setRatesTo-java.util.Date-) | Imposta l'ultima data in cui una tariffa è effettiva. |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | Imposta la tariffa standard per ora per una risorsa. |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | Imposta le unità utilizzate da Microsoft Project per visualizzare la tariffa standard. |
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


Ottiene il costo per utilizzo di una risorsa. Questo valore viene recuperato dalla data corrente se esiste una tabella delle tariffe per una risorsa.

**Returns:**
java.math.BigDecimal - il costo per utilizzo di una risorsa.
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


Ottiene la tariffa degli straordinari per ora per una risorsa.

**Returns:**
java.math.BigDecimal - la tariffa degli straordinari per ora per una risorsa.
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


Ottiene le unità utilizzate da Microsoft Project per visualizzare la tariffa degli straordinari.

**Returns:**
int - le unità utilizzate da Microsoft Project per visualizzare la tariffa degli straordinari.
### getRateTable() {#getRateTable--}
```
public final int getRateTable()
```


Ottiene l'identificatore univoco di una tabella delle tariffe per una risorsa.

**Returns:**
int - l'identificatore univoco di una tabella delle tariffe per una risorsa.
### getRatesFrom() {#getRatesFrom--}
```
public final Date getRatesFrom()
```


Ottiene la data in cui una tariffa entra in vigore.

**Returns:**
java.util.Date - la data in cui una tariffa diventa effettiva.
### getRatesTo() {#getRatesTo--}
```
public final Date getRatesTo()
```


Ottiene l'ultima data in cui una tariffa è valida.

**Returns:**
java.util.Date - l'ultima data in cui una tariffa è effettiva.
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


Ottiene la tariffa standard per ora per una risorsa.

**Returns:**
java.math.BigDecimal - la tariffa standard per ora per una risorsa.
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


Ottiene le unità utilizzate da Microsoft Project per visualizzare la tariffa standard.

**Returns:**
int - le unità utilizzate da Microsoft Project per visualizzare la tariffa standard.
### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


Imposta il costo per utilizzo di una risorsa. Questo valore viene recuperato dalla data corrente se esiste una tabella delle tariffe per una risorsa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.math.BigDecimal | il costo per utilizzo di una risorsa. |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


Imposta la tariffa degli straordinari per ora per una risorsa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.math.BigDecimal | la tariffa degli straordinari per ora per una risorsa. |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


Imposta le unità utilizzate da Microsoft Project per visualizzare la tariffa degli straordinari.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | le unità utilizzate da Microsoft Project per visualizzare la tariffa degli straordinari. |

### setRateTable(int value) {#setRateTable-int-}
```
public final void setRateTable(int value)
```


Imposta l'identificatore univoco di una tabella delle tariffe per una risorsa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | l'identificatore univoco di una tabella delle tariffe per una risorsa. |

### setRatesFrom(Date value) {#setRatesFrom-java.util.Date-}
```
public final void setRatesFrom(Date value)
```


Imposta la data in cui una tariffa diventa effettiva.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | la data in cui una tariffa diventa effettiva. |

### setRatesTo(Date value) {#setRatesTo-java.util.Date-}
```
public final void setRatesTo(Date value)
```


Imposta l'ultima data in cui una tariffa è effettiva.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | l'ultima data in cui una tariffa è effettiva. |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


Imposta la tariffa standard per ora per una risorsa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.math.BigDecimal | la tariffa standard per ora per una risorsa. |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


Imposta le unità utilizzate da Microsoft Project per visualizzare la tariffa standard.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | le unità utilizzate da Microsoft Project per visualizzare la tariffa standard. |

