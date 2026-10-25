---
title: "RiskItemStatistics"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar ett objekt som lagrar statistiska data för uppgiften i det analyserade projektet."
type: docs
weight: 265
url: /sv/java/com.aspose.tasks/riskitemstatistics/
---

**Inheritance:**
java.lang.Object
```
public class RiskItemStatistics
```

Representerar ett objekt som lagrar statistiska data för uppgiften i det analyserade projektet.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getExpectedValue()](#getExpectedValue--) | Hämtar det förväntade värdet för riskobjektet. |
| [getItemType()](#getItemType--) | Hämtar en instans av [RiskItemType](../../com.aspose.tasks/riskitemtype)-enumerationen. |
| [getMaximum()](#getMaximum--) | Hämtar det maximala värdet som genererades under Monte Carlo-simulering. |
| [getMinimum()](#getMinimum--) | Hämtar det minimala värdet som genererades under Monte Carlo-simulering. |
| [getPercentile(int percent)](#getPercentile-int-) | Hämtar ett värde under vilket en angiven procentandel av de genererade proverna faller. |
| [getStandardDeviation()](#getStandardDeviation--) | Hämtar standardavvikelsen för riskobjektet. |
| [toString()](#toString--) | Returnerar en kort strängrepresentation av ett riskobjekt. |
### getExpectedValue() {#getExpectedValue--}
```
public final Date getExpectedValue()
```


Hämtar det förväntade värdet för riskobjektet.

**Returns:**
java.util.Date - det förväntade värdet för riskobjektet.
### getItemType() {#getItemType--}
```
public final int getItemType()
```


Hämtar en instans av [RiskItemType](../../com.aspose.tasks/riskitemtype)-enumerationen.

**Returns:**
int - en instans av [RiskItemType](../../com.aspose.tasks/riskitemtype)-enumerationen.
### getMaximum() {#getMaximum--}
```
public final Date getMaximum()
```


Hämtar det maximala värdet som genererades under Monte Carlo-simulering.

**Returns:**
java.util.Date - det maximala värdet som genererades under Monte Carlo-simulering.
### getMinimum() {#getMinimum--}
```
public final Date getMinimum()
```


Hämtar det minimala värdet som genererades under Monte Carlo-simulering.

**Returns:**
java.util.Date - det minimala värdet som genererades under Monte Carlo-simulering.
### getPercentile(int percent) {#getPercentile-int-}
```
public final Date getPercentile(int percent)
```


Hämtar ett värde under vilket en angiven procentandel av de genererade proverna faller.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| procent | int | den angivna procenten mellan 0 och 100. |

**Returns:**
java.util.Date - ett värde under vilket en angiven procentandel av de genererade proverna faller.
### getStandardDeviation() {#getStandardDeviation--}
```
public final Duration getStandardDeviation()
```


Hämtar standardavvikelsen för riskobjektet.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the standard deviation of the risk item.
### toString() {#toString--}
```
public String toString()
```


Returnerar en kort strängrepresentation av ett riskobjekt. De exakta detaljerna för representationen är ospecificerade och kan förändras.

**Returns:**
java.lang.String - kort sträng som representerar RiskItem-objektet.
