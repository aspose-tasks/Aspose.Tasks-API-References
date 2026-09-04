---
title: "RiskAnalysisResult"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt ein Ergebnis der Risikoanalyse dar."
type: docs
weight: 262
url: /de/java/com.aspose.tasks/riskanalysisresult/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalysisResult
```

Stellt ein Ergebnis der Risikoanalyse dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getRiskItems(int itemType)](#getRiskItems-int-) | Gibt eine Instanz von [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) für den angegebenen Risikotyp zurück. |
| [saveReport(InputStream stream)](#saveReport-java.io.InputStream-) | Speichert den Risikoanalysebericht im Stream im PDF-Format. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | Speichert den Risikoanalysebericht im angegebenen Dateipfad im PDF-Format. |
### getRiskItems(int itemType) {#getRiskItems-int-}
```
public final RiskItemStatisticsCollection getRiskItems(int itemType)
```


Gibt eine Instanz von [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) für den angegebenen Risikotyp zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| itemType | int | der angegebene Risikotyp; kann einer der Werte der [RiskItemType](../../com.aspose.tasks/riskitemtype)-Aufzählung sein. |

**Returns:**
[RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) - an instance of the [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) for the specified risk type.
### saveReport(InputStream stream) {#saveReport-java.io.InputStream-}
```
public final void saveReport(InputStream stream)
```


Speichert den Risikoanalysebericht im Stream im PDF-Format.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.InputStream | Der Stream, in dem der Risikoanalysebericht gespeichert werden soll. |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


Speichert den Risikoanalysebericht im angegebenen Dateipfad im PDF-Format.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der angegebene Dateiname. |

