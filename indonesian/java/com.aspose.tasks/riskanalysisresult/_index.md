---
title: "RiskAnalysisResult"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili hasil analisis risiko."
type: docs
weight: 262
url: /id/java/com.aspose.tasks/riskanalysisresult/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalysisResult
```

Mewakili hasil analisis risiko.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getRiskItems(int itemType)](#getRiskItems-int-) | Mengembalikan sebuah instance dari [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) untuk tipe risiko yang ditentukan. |
| [saveReport(InputStream stream)](#saveReport-java.io.InputStream-) | Menyimpan laporan analisis risiko ke aliran dalam format PDF. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | Menyimpan laporan analisis risiko ke jalur file yang ditentukan dalam format PDF. |
### getRiskItems(int itemType) {#getRiskItems-int-}
```
public final RiskItemStatisticsCollection getRiskItems(int itemType)
```


Mengembalikan sebuah instance dari [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) untuk tipe risiko yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| itemType | int | tipe risiko yang ditentukan; dapat berupa salah satu nilai dari enumerasi [RiskItemType](../../com.aspose.tasks/riskitemtype). |

**Returns:**
[RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) - an instance of the [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) for the specified risk type.
### saveReport(InputStream stream) {#saveReport-java.io.InputStream-}
```
public final void saveReport(InputStream stream)
```


Menyimpan laporan analisis risiko ke aliran dalam format PDF.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.InputStream | Aliran untuk menyimpan laporan analisis risiko. |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


Menyimpan laporan analisis risiko ke jalur file yang ditentukan dalam format PDF.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | java.lang.String | Nama file yang ditentukan. |

