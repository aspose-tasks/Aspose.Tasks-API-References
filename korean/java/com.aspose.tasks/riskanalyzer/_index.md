---
title: "RiskAnalyzer"
second_title: "Aspose.Tasks for Java API Reference"
description: "지정된 위험 분석 설정을 기반으로 몬테카를로 시뮬레이션을 수행합니다."
type: docs
weight: 264
url: /ko/java/com.aspose.tasks/riskanalyzer/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalyzer
```

지정된 위험 분석 설정을 기반으로 몬테카를로 시뮬레이션을 수행합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [RiskAnalyzer(RiskAnalysisSettings settings)](#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-) | [RiskAnalyzer](../../com.aspose.tasks/riskanalyzer) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [analyze(Project project)](#analyze-com.aspose.tasks.Project-) | 지정된 프로젝트에 대한 위험 분석을 수행합니다. |
| [getSettings()](#getSettings--) | 위험 분석에 필요한 설정을 정의하는 [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) 클래스의 인스턴스를 가져옵니다. |
| [setSettings(RiskAnalysisSettings value)](#setSettings-com.aspose.tasks.RiskAnalysisSettings-) | 위험 분석에 필요한 설정을 정의하는 [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) 클래스의 인스턴스를 설정합니다. |
### RiskAnalyzer(RiskAnalysisSettings settings) {#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-}
```
public RiskAnalyzer(RiskAnalysisSettings settings)
```


[RiskAnalyzer](../../com.aspose.tasks/riskanalyzer) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| settings | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) 클래스의 지정된 인스턴스입니다. |

### analyze(Project project) {#analyze-com.aspose.tasks.Project-}
```
public final RiskAnalysisResult analyze(Project project)
```


지정된 프로젝트에 대한 위험 분석을 수행합니다. 분석은 몬테카를로 시뮬레이션을 기반으로 하며 결과는 [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) 클래스의 인스턴스입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | 분석할 [Project](../../com.aspose.tasks/project) 클래스의 지정된 인스턴스. |

**Returns:**
[RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) - the instance of the [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) which represents a result of the analysis.
### getSettings() {#getSettings--}
```
public final RiskAnalysisSettings getSettings()
```


위험 분석에 필요한 설정을 정의하는 [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) 클래스의 인스턴스를 가져옵니다.

**Returns:**
[RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) - the instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class which defines necessary settings for risk analysis.
### setSettings(RiskAnalysisSettings value) {#setSettings-com.aspose.tasks.RiskAnalysisSettings-}
```
public final void setSettings(RiskAnalysisSettings value)
```


위험 분석에 필요한 설정을 정의하는 [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) 클래스의 인스턴스를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | 위험 분석에 필요한 설정을 정의하는 [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) 클래스의 인스턴스. |

