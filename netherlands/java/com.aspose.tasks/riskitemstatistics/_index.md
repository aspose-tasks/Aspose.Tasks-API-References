---
title: "RiskItemStatistics"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Vertegenwoordigt een item dat statistische gegevens opslaat voor de taak van het geanalyseerde project."
type: docs
weight: 265
url: /nl/java/com.aspose.tasks/riskitemstatistics/
---

**Inheritance:**
java.lang.Object
```
public class RiskItemStatistics
```

Vertegenwoordigt een item dat statistische gegevens opslaat voor de taak van het geanalyseerde project.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getExpectedValue()](#getExpectedValue--) | Haalt de verwachte waarde van het risicoelement op. |
| [getItemType()](#getItemType--) | Haalt een instantie van de [RiskItemType](../../com.aspose.tasks/riskitemtype) enumeratie op. |
| [getMaximum()](#getMaximum--) | Haalt de maximale waarde op die tijdens de Monte Carlo-simulatie is gegenereerd. |
| [getMinimum()](#getMinimum--) | Haalt de minimale waarde op die tijdens de Monte Carlo-simulatie is gegenereerd. |
| [getPercentile(int percent)](#getPercentile-int-) | Haalt een waarde op waaronder een opgegeven percentage van de gegenereerde monsters valt. |
| [getStandardDeviation()](#getStandardDeviation--) | Haalt de standaarddeviatie van het risicoelement op. |
| [toString()](#toString--) | Retourneert een korte tekenreeksrepresentatie van een risicoelement. |
### getExpectedValue() {#getExpectedValue--}
```
public final Date getExpectedValue()
```


Haalt de verwachte waarde van het risicoelement op.

**Returns:**
java.util.Date - de verwachte waarde van het risicoelement.
### getItemType() {#getItemType--}
```
public final int getItemType()
```


Haalt een instantie van de [RiskItemType](../../com.aspose.tasks/riskitemtype) enumeratie op.

**Returns:**
int - een instantie van de [RiskItemType](../../com.aspose.tasks/riskitemtype) enumeratie.
### getMaximum() {#getMaximum--}
```
public final Date getMaximum()
```


Haalt de maximale waarde op die tijdens de Monte Carlo-simulatie is gegenereerd.

**Returns:**
java.util.Date - de maximale waarde die tijdens de Monte Carlo-simulatie werd gegenereerd.
### getMinimum() {#getMinimum--}
```
public final Date getMinimum()
```


Haalt de minimale waarde op die tijdens de Monte Carlo-simulatie is gegenereerd.

**Returns:**
java.util.Date - de minimale waarde die tijdens de Monte Carlo-simulatie werd gegenereerd.
### getPercentile(int percent) {#getPercentile-int-}
```
public final Date getPercentile(int percent)
```


Haalt een waarde op waaronder een opgegeven percentage van de gegenereerde monsters valt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| percentage | int | het opgegeven percentage tussen 0 en 100. |

**Returns:**
java.util.Date - een waarde waaronder een opgegeven percentage van de gegenereerde monsters valt.
### getStandardDeviation() {#getStandardDeviation--}
```
public final Duration getStandardDeviation()
```


Haalt de standaarddeviatie van het risicoelement op.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the standard deviation of the risk item.
### toString() {#toString--}
```
public String toString()
```


Retourneert een korte tekenreeksrepresentatie van een risicoelement. De exacte details van de representatie zijn niet gespecificeerd en kunnen wijzigen.

**Returns:**
java.lang.String - korte tekenreeks die een RiskItem-object representeert.
