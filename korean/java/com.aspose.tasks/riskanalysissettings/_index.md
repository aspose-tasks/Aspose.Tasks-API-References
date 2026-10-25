---
title: "RiskAnalysisSettings"
second_title: "Aspose.Tasks for Java API Reference"
description: "위험 분석 수행을 위한 설정을 지정합니다."
type: docs
weight: 263
url: /ko/java/com.aspose.tasks/riskanalysissettings/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalysisSettings
```

위험 분석 수행을 위한 설정을 지정합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [RiskAnalysisSettings()](#RiskAnalysisSettings--) | 새로운 [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getIterationsCount()](#getIterationsCount--) | Monte Carlo 시뮬레이션에 사용할 반복 횟수를 가져옵니다. |
| [getPatterns()](#getPatterns--) | [RiskPattern](../../com.aspose.tasks/riskpattern) 클래스 인스턴스를 포함하는 컬렉션을 가져옵니다. |
| [setIterationsCount(int value)](#setIterationsCount-int-) | Monte Carlo 시뮬레이션에 사용할 반복 횟수를 설정합니다. |
### RiskAnalysisSettings() {#RiskAnalysisSettings--}
```
public RiskAnalysisSettings()
```


새로운 [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) 클래스 인스턴스를 초기화합니다.

### getIterationsCount() {#getIterationsCount--}
```
public final int getIterationsCount()
```


Monte Carlo 시뮬레이션에 사용할 반복 횟수를 가져옵니다. 기본값은 100입니다.

**Returns:**
int - Monte Carlo 시뮬레이션에 사용할 반복 횟수.
### getPatterns() {#getPatterns--}
```
public final RiskPatternCollection getPatterns()
```


[RiskPattern](../../com.aspose.tasks/riskpattern) 클래스 인스턴스를 포함하는 컬렉션을 가져옵니다.

**Returns:**
[RiskPatternCollection](../../com.aspose.tasks/riskpatterncollection) - a collection containing the instances of the [RiskPattern](../../com.aspose.tasks/riskpattern) class.
### setIterationsCount(int value) {#setIterationsCount-int-}
```
public final void setIterationsCount(int value)
```


Monte Carlo 시뮬레이션에 사용할 반복 횟수를 설정합니다. 기본값은 100입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 몬테카를로 시뮬레이션에 사용할 반복 횟수. |

