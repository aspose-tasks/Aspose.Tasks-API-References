---
title: "RiskAnalyzer"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Melakukan simulasi Monte Carlo berdasarkan pengaturan analisis risiko yang ditentukan."
type: docs
weight: 264
url: /id/java/com.aspose.tasks/riskanalyzer/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalyzer
```

Melakukan simulasi Monte Carlo berdasarkan pengaturan analisis risiko yang ditentukan.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [RiskAnalyzer(RiskAnalysisSettings settings)](#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-) | Menginisialisasi sebuah instance baru dari kelas [RiskAnalyzer](../../com.aspose.tasks/riskanalyzer). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [analyze(Project project)](#analyze-com.aspose.tasks.Project-) | Melakukan analisis risiko untuk proyek yang ditentukan. |
| [getSettings()](#getSettings--) | Mendapatkan instance dari kelas [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) yang mendefinisikan pengaturan yang diperlukan untuk analisis risiko. |
| [setSettings(RiskAnalysisSettings value)](#setSettings-com.aspose.tasks.RiskAnalysisSettings-) | Mengatur instance dari kelas [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) yang mendefinisikan pengaturan yang diperlukan untuk analisis risiko. |
### RiskAnalyzer(RiskAnalysisSettings settings) {#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-}
```
public RiskAnalyzer(RiskAnalysisSettings settings)
```


Menginisialisasi sebuah instance baru dari kelas [RiskAnalyzer](../../com.aspose.tasks/riskanalyzer).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| settings | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | instance yang ditentukan dari kelas [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings). |

### analyze(Project project) {#analyze-com.aspose.tasks.Project-}
```
public final RiskAnalysisResult analyze(Project project)
```


Melakukan analisis risiko untuk proyek yang ditentukan. Analisis ini didasarkan pada simulasi Monte Carlo dan hasilnya adalah sebuah instance dari kelas [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | instance yang ditentukan dari kelas [Project](../../com.aspose.tasks/project) untuk dianalisis. |

**Returns:**
[RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) - the instance of the [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) which represents a result of the analysis.
### getSettings() {#getSettings--}
```
public final RiskAnalysisSettings getSettings()
```


Mendapatkan instance dari kelas [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) yang mendefinisikan pengaturan yang diperlukan untuk analisis risiko.

**Returns:**
[RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) - the instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class which defines necessary settings for risk analysis.
### setSettings(RiskAnalysisSettings value) {#setSettings-com.aspose.tasks.RiskAnalysisSettings-}
```
public final void setSettings(RiskAnalysisSettings value)
```


Mengatur instance dari kelas [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) yang mendefinisikan pengaturan yang diperlukan untuk analisis risiko.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | instance dari kelas [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) yang mendefinisikan pengaturan yang diperlukan untuk analisis risiko. |

