---
title: "RiskItemStatistics"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt ein Element dar, das statistische Daten für die Aufgabe des analysierten Projekts speichert."
type: docs
weight: 265
url: /de/java/com.aspose.tasks/riskitemstatistics/
---

**Inheritance:**
java.lang.Object
```
public class RiskItemStatistics
```

Stellt ein Element dar, das statistische Daten für die Aufgabe des analysierten Projekts speichert.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getExpectedValue()](#getExpectedValue--) | Liefert den erwarteten Wert des Risiko‑Elements. |
| [getItemType()](#getItemType--) | Liefert eine Instanz der [RiskItemType](../../com.aspose.tasks/riskitemtype)-Aufzählung. |
| [getMaximum()](#getMaximum--) | Liefert den maximalen Wert, der während der Monte‑Carlo‑Simulation erzeugt wurde. |
| [getMinimum()](#getMinimum--) | Liefert den minimalen Wert, der während der Monte‑Carlo‑Simulation erzeugt wurde. |
| [getPercentile(int percent)](#getPercentile-int-) | Liefert einen Wert, unter dem ein bestimmter Prozentsatz der erzeugten Stichproben liegt. |
| [getStandardDeviation()](#getStandardDeviation--) | Liefert die Standardabweichung des Risiko‑Elements. |
| [toString()](#toString--) | Gibt eine kurze Zeichenketten‑Darstellung eines Risiko‑Elements zurück. |
### getExpectedValue() {#getExpectedValue--}
```
public final Date getExpectedValue()
```


Liefert den erwarteten Wert des Risiko‑Elements.

**Returns:**
java.util.Date - der erwartete Wert des Risiko‑Elements.
### getItemType() {#getItemType--}
```
public final int getItemType()
```


Liefert eine Instanz der [RiskItemType](../../com.aspose.tasks/riskitemtype)-Aufzählung.

**Returns:**
int - eine Instanz der [RiskItemType](../../com.aspose.tasks/riskitemtype)-Aufzählung.
### getMaximum() {#getMaximum--}
```
public final Date getMaximum()
```


Liefert den maximalen Wert, der während der Monte‑Carlo‑Simulation erzeugt wurde.

**Returns:**
java.util.Date - der maximale Wert, der während der Monte‑Carlo‑Simulation erzeugt wurde.
### getMinimum() {#getMinimum--}
```
public final Date getMinimum()
```


Liefert den minimalen Wert, der während der Monte‑Carlo‑Simulation erzeugt wurde.

**Returns:**
java.util.Date - der minimale Wert, der während der Monte‑Carlo‑Simulation erzeugt wurde.
### getPercentile(int percent) {#getPercentile-int-}
```
public final Date getPercentile(int percent)
```


Liefert einen Wert, unter dem ein bestimmter Prozentsatz der erzeugten Stichproben liegt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Prozent | int | der angegebene Prozentsatz zwischen 0 und 100. |

**Returns:**
java.util.Date - ein Wert, unter dem ein bestimmter Prozentsatz der erzeugten Stichproben liegt.
### getStandardDeviation() {#getStandardDeviation--}
```
public final Duration getStandardDeviation()
```


Liefert die Standardabweichung des Risiko‑Elements.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the standard deviation of the risk item.
### toString() {#toString--}
```
public String toString()
```


Gibt eine kurze Zeichenketten‑Darstellung eines Risiko‑Elements zurück. Die genauen Details der Darstellung sind nicht spezifiziert und können sich ändern.

**Returns:**
java.lang.String - kurze Zeichenkette, die das RiskItem‑Objekt darstellt.
