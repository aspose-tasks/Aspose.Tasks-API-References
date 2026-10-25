---
title: "RiskAnalyzer"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "ينفّذ محاكاة مونت كارلو بناءً على إعدادات تحليل المخاطر المحددة."
type: docs
weight: 264
url: /ar/java/com.aspose.tasks/riskanalyzer/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalyzer
```

ينفّذ محاكاة مونت كارلو بناءً على إعدادات تحليل المخاطر المحددة.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [RiskAnalyzer(RiskAnalysisSettings settings)](#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-) | ينشئ مثيلاً جديدًا من الفئة [RiskAnalyzer](../../com.aspose/tasks/riskanalyzer) class. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [analyze(Project project)](#analyze-com.aspose.tasks.Project-) | يُجري تحليل المخاطر للمشروع المحدد. |
| [getSettings()](#getSettings--) | يحصل على مثيل الفئة [RiskAnalysisSettings](../../com.aspose/tasks/riskanalysissettings) class التي تحدد الإعدادات اللازمة لتحليل المخاطر. |
| [setSettings(RiskAnalysisSettings value)](#setSettings-com.aspose.tasks.RiskAnalysisSettings-) | يضبط مثيل الفئة [RiskAnalysisSettings](../../com.aspose/tasks/riskanalysissettings) class التي تحدد الإعدادات اللازمة لتحليل المخاطر. |
### RiskAnalyzer(RiskAnalysisSettings settings) {#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-}
```
public RiskAnalyzer(RiskAnalysisSettings settings)
```


ينشئ مثيلاً جديدًا من الفئة [RiskAnalyzer](../../com.aspose/tasks/riskanalyzer) class.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| settings | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | المثيل المحدد للفئة [RiskAnalysisSettings](../../com.aspose/tasks/riskanalysissettings) class. |

### analyze(Project project) {#analyze-com.aspose.tasks.Project-}
```
public final RiskAnalysisResult analyze(Project project)
```


يُجري تحليل المخاطر للمشروع المحدد. يعتمد التحليل على محاكاة مونت كارلو والنتيجة هي مثيل الفئة [RiskAnalysisResult](../../com.aspose/tasks/riskanalysisresult) class.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | المثيل المحدد للفئة [Project](../../com.aspose/tasks/project) class للتحليل. |

**Returns:**
[RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) - the instance of the [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) which represents a result of the analysis.
### getSettings() {#getSettings--}
```
public final RiskAnalysisSettings getSettings()
```


يحصل على مثيل الفئة [RiskAnalysisSettings](../../com.aspose/tasks/riskanalysissettings) class التي تحدد الإعدادات اللازمة لتحليل المخاطر.

**Returns:**
[RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) - the instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class which defines necessary settings for risk analysis.
### setSettings(RiskAnalysisSettings value) {#setSettings-com.aspose.tasks.RiskAnalysisSettings-}
```
public final void setSettings(RiskAnalysisSettings value)
```


يضبط مثيل الفئة [RiskAnalysisSettings](../../com.aspose/tasks/riskanalysissettings) class التي تحدد الإعدادات اللازمة لتحليل المخاطر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | مثيل الفئة [RiskAnalysisSettings](../../com.aspose/tasks/riskanalysissettings) class التي تحدد الإعدادات اللازمة لتحليل المخاطر. |

