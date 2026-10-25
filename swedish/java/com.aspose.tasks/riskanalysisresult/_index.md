---
title: "RiskAnalysisResult"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar ett resultat av riskanalys."
type: docs
weight: 262
url: /sv/java/com.aspose.tasks/riskanalysisresult/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalysisResult
```

Representerar ett resultat av riskanalys.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getRiskItems(int itemType)](#getRiskItems-int-) | Returnerar en instans av [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) för den angivna risktypen. |
| [saveReport(InputStream stream)](#saveReport-java.io.InputStream-) | Sparar riskanalysrapporten till strömmen i PDF-format. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | Sparar riskanalysrapporten till den angivna filsökvägen i PDF-format. |
### getRiskItems(int itemType) {#getRiskItems-int-}
```
public final RiskItemStatisticsCollection getRiskItems(int itemType)
```


Returnerar en instans av [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) för den angivna risktypen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| itemType | int | den angivna risktypen; kan vara ett av värdena i uppräkningen [RiskItemType](../../com.aspose.tasks/riskitemtype). |

**Returns:**
[RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) - an instance of the [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) for the specified risk type.
### saveReport(InputStream stream) {#saveReport-java.io.InputStream-}
```
public final void saveReport(InputStream stream)
```


Sparar riskanalysrapporten till strömmen i PDF-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.InputStream | Strömmen att spara riskanalysrapporten till. |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


Sparar riskanalysrapporten till den angivna filsökvägen i PDF-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | Det angivna filnamnet. |

