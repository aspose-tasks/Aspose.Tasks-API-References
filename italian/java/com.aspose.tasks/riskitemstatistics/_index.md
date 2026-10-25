---
title: "RiskItemStatistics"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un elemento che memorizza i dati statistici per l'attività del progetto analizzato."
type: docs
weight: 265
url: /it/java/com.aspose.tasks/riskitemstatistics/
---

**Inheritance:**
java.lang.Object
```
public class RiskItemStatistics
```

Rappresenta un elemento che memorizza i dati statistici per l'attività del progetto analizzato.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getExpectedValue()](#getExpectedValue--) | Restituisce il valore atteso dell'elemento di rischio. |
| [getItemType()](#getItemType--) | Restituisce un'istanza dell'enumerazione [RiskItemType](../../com.aspose.tasks/riskitemtype). |
| [getMaximum()](#getMaximum--) | Restituisce il valore massimo generato durante la simulazione Monte Carlo. |
| [getMinimum()](#getMinimum--) | Restituisce il valore minimo generato durante la simulazione Monte Carlo. |
| [getPercentile(int percent)](#getPercentile-int-) | Restituisce un valore al di sotto del quale cade una percentuale specificata di campioni generati. |
| [getStandardDeviation()](#getStandardDeviation--) | Restituisce la deviazione standard dell'elemento di rischio. |
| [toString()](#toString--) | Restituisce la rappresentazione stringa breve di un elemento di rischio. |
### getExpectedValue() {#getExpectedValue--}
```
public final Date getExpectedValue()
```


Restituisce il valore atteso dell'elemento di rischio.

**Returns:**
java.util.Date - il valore previsto dell'elemento di rischio.
### getItemType() {#getItemType--}
```
public final int getItemType()
```


Restituisce un'istanza dell'enumerazione [RiskItemType](../../com.aspose.tasks/riskitemtype).

**Returns:**
int - un'istanza dell'enumerazione [RiskItemType](../../com.aspose.tasks/riskitemtype).
### getMaximum() {#getMaximum--}
```
public final Date getMaximum()
```


Restituisce il valore massimo generato durante la simulazione Monte Carlo.

**Returns:**
java.util.Date - il valore massimo generato durante la simulazione Monte Carlo.
### getMinimum() {#getMinimum--}
```
public final Date getMinimum()
```


Restituisce il valore minimo generato durante la simulazione Monte Carlo.

**Returns:**
java.util.Date - il valore minimo generato durante la simulazione Monte Carlo.
### getPercentile(int percent) {#getPercentile-int-}
```
public final Date getPercentile(int percent)
```


Restituisce un valore al di sotto del quale cade una percentuale specificata di campioni generati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percentuale | int | la percentuale specificata tra 0 e 100. |

**Returns:**
java.util.Date - un valore al di sotto del quale cade una percentuale specificata di campioni generati.
### getStandardDeviation() {#getStandardDeviation--}
```
public final Duration getStandardDeviation()
```


Restituisce la deviazione standard dell'elemento di rischio.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the standard deviation of the risk item.
### toString() {#toString--}
```
public String toString()
```


Restituisce la rappresentazione in forma di stringa breve di un elemento di rischio. I dettagli esatti della rappresentazione non sono specificati e possono cambiare.

**Returns:**
java.lang.String - stringa breve che rappresenta l'oggetto RiskItem.
