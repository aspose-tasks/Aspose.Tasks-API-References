---
title: "RiskAnalyzer"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Belirtilen risk analizi ayarlarına dayalı bir Monte Carlo simülasyonu gerçekleştirir."
type: docs
weight: 264
url: /tr/java/com.aspose.tasks/riskanalyzer/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalyzer
```

Belirtilen risk analizi ayarlarına dayalı bir Monte Carlo simülasyonu gerçekleştirir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [RiskAnalyzer(RiskAnalysisSettings settings)](#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-) | Yeni bir [RiskAnalyzer](../../com.aspose.tasks/riskanalyzer) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [analyze(Project project)](#analyze-com.aspose.tasks.Project-) | Belirtilen proje için risk analizini gerçekleştirir. |
| [getSettings()](#getSettings--) | Risk analizi için gerekli ayarları tanımlayan [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) sınıfının örneğini alır. |
| [setSettings(RiskAnalysisSettings value)](#setSettings-com.aspose.tasks.RiskAnalysisSettings-) | Risk analizi için gerekli ayarları tanımlayan [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) sınıfının örneğini ayarlar. |
### RiskAnalyzer(RiskAnalysisSettings settings) {#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-}
```
public RiskAnalyzer(RiskAnalysisSettings settings)
```


Yeni bir [RiskAnalyzer](../../com.aspose.tasks/riskanalyzer) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| settings | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | Belirtilen [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) sınıfı örneği. |

### analyze(Project project) {#analyze-com.aspose.tasks.Project-}
```
public final RiskAnalysisResult analyze(Project project)
```


Belirtilen proje için risk analizini gerçekleştirir. Analiz Monte Carlo simülasyonuna dayanır ve sonuç bir [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) sınıfı örneğidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Analiz edilecek belirtilen [Project](../../com.aspose.tasks/project) sınıfı örneği. |

**Returns:**
[RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) - the instance of the [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) which represents a result of the analysis.
### getSettings() {#getSettings--}
```
public final RiskAnalysisSettings getSettings()
```


Risk analizi için gerekli ayarları tanımlayan [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) sınıfının örneğini alır.

**Returns:**
[RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) - the instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class which defines necessary settings for risk analysis.
### setSettings(RiskAnalysisSettings value) {#setSettings-com.aspose.tasks.RiskAnalysisSettings-}
```
public final void setSettings(RiskAnalysisSettings value)
```


Risk analizi için gerekli ayarları tanımlayan [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) sınıfının örneğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | Risk analizi için gerekli ayarları tanımlayan [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) sınıfının örneği. |

