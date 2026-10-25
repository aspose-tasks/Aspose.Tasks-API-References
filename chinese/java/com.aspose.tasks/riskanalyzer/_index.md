---
title: "RiskAnalyzer"
second_title: "Aspose.Tasks for Java API 参考"
description: "根据指定的风险分析设置执行蒙特卡罗模拟。"
type: docs
weight: 264
url: /zh/java/com.aspose.tasks/riskanalyzer/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalyzer
```

根据指定的风险分析设置执行蒙特卡罗模拟。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [RiskAnalyzer(RiskAnalysisSettings settings)](#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-) | 初始化一个新的 [RiskAnalyzer](../../com.aspose.tasks/riskanalyzer) 类实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [analyze(Project project)](#analyze-com.aspose.tasks.Project-) | 对指定项目执行风险分析。 |
| [getSettings()](#getSettings--) | 获取 [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) 类的实例，该实例定义了风险分析所需的设置。 |
| [setSettings(RiskAnalysisSettings value)](#setSettings-com.aspose.tasks.RiskAnalysisSettings-) | 设置 [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) 类的实例，该实例定义了风险分析所需的设置。 |
### RiskAnalyzer(RiskAnalysisSettings settings) {#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-}
```
public RiskAnalyzer(RiskAnalysisSettings settings)
```


初始化一个新的 [RiskAnalyzer](../../com.aspose.tasks/riskanalyzer) 类实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| settings | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | 指定的 [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) 类实例。 |

### analyze(Project project) {#analyze-com.aspose.tasks.Project-}
```
public final RiskAnalysisResult analyze(Project project)
```


对指定项目执行风险分析。该分析基于蒙特卡罗模拟，结果是 [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) 类的实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | 要分析的 [Project](../../com.aspose.tasks/project) 类的指定实例。 |

**Returns:**
[RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) - the instance of the [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) which represents a result of the analysis.
### getSettings() {#getSettings--}
```
public final RiskAnalysisSettings getSettings()
```


获取 [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) 类的实例，该实例定义了风险分析所需的设置。

**Returns:**
[RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) - the instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class which defines necessary settings for risk analysis.
### setSettings(RiskAnalysisSettings value) {#setSettings-com.aspose.tasks.RiskAnalysisSettings-}
```
public final void setSettings(RiskAnalysisSettings value)
```


设置 [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) 类的实例，该实例定义了风险分析所需的设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | 用于定义风险分析必要设置的 [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) 类的实例。 |

