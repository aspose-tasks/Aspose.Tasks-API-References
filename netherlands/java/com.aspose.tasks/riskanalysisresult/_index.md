---
title: "RiskAnalysisResult"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Vertegenwoordigt een resultaat van risicoanalyse."
type: docs
weight: 262
url: /nl/java/com.aspose.tasks/riskanalysisresult/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalysisResult
```

Vertegenwoordigt een resultaat van risicoanalyse.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getRiskItems(int itemType)](#getRiskItems-int-) | Retourneert een instantie van de [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) voor het opgegeven risicotype. |
| [saveReport(InputStream stream)](#saveReport-java.io.InputStream-) | Slaat het risico‑analyse‑rapport op naar de stream in PDF‑formaat. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | Slaat het risico‑analyse‑rapport op naar het opgegeven bestandspad in PDF‑formaat. |
### getRiskItems(int itemType) {#getRiskItems-int-}
```
public final RiskItemStatisticsCollection getRiskItems(int itemType)
```


Retourneert een instantie van de [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) voor het opgegeven risicotype.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| itemType | int | het opgegeven risicotype; kan een van de waarden van de [RiskItemType](../../com.aspose.tasks/riskitemtype) enumeratie zijn. |

**Returns:**
[RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) - an instance of the [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) for the specified risk type.
### saveReport(InputStream stream) {#saveReport-java.io.InputStream-}
```
public final void saveReport(InputStream stream)
```


Slaat het risico‑analyse‑rapport op naar de stream in PDF‑formaat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | java.io.InputStream | De stream waarin het risico‑analyse‑rapport moet worden opgeslagen. |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


Slaat het risico‑analyse‑rapport op naar het opgegeven bestandspad in PDF‑formaat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | java.lang.String | De opgegeven bestandsnaam. |

