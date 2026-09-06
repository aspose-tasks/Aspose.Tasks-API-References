---
title: "RiskAnalysisResult"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Risk analizinin sonucunu temsil eder."
type: docs
weight: 262
url: /tr/java/com.aspose.tasks/riskanalysisresult/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalysisResult
```

Risk analizinin sonucunu temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getRiskItems(int itemType)](#getRiskItems-int-) | Belirtilen risk türü için [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) örneği döndürür. |
| [saveReport(InputStream stream)](#saveReport-java.io.InputStream-) | Risk analiz raporunu PDF formatında akışa kaydeder. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | Risk analiz raporunu belirtilen dosya yoluna PDF formatında kaydeder. |
### getRiskItems(int itemType) {#getRiskItems-int-}
```
public final RiskItemStatisticsCollection getRiskItems(int itemType)
```


Belirtilen risk türü için [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) örneği döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| itemType | int | belirtilen risk türü; [RiskItemType](../../com.aspose.tasks/riskitemtype) sayımının değerlerinden biri olabilir. |

**Returns:**
[RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) - an instance of the [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) for the specified risk type.
### saveReport(InputStream stream) {#saveReport-java.io.InputStream-}
```
public final void saveReport(InputStream stream)
```


Risk analiz raporunu PDF formatında akışa kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.InputStream | Risk analiz raporunun kaydedileceği akış. |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


Risk analiz raporunu belirtilen dosya yoluna PDF formatında kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | Belirtilen dosya adı. |

