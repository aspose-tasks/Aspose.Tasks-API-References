---
title: "RiskPattern"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트 작업에 대한 위험 패턴을 나타냅니다."
type: docs
weight: 268
url: /ko/java/com.aspose.tasks/riskpattern/
---

**Inheritance:**
java.lang.Object
```
public class RiskPattern
```

프로젝트 작업에 대한 위험 패턴을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [RiskPattern(Task task)](#RiskPattern-com.aspose.tasks.Task-) | 새 인스턴스를 초기화합니다 [RiskPattern](../../com.aspose.tasks/riskpattern) 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getConfidenceLevel()](#getConfidenceLevel--) | 실제 생성된 값이 낙관적 및 비관적 추정치 범위 내에 있을 확률 비율에 해당하는 신뢰 수준을 가져옵니다. |
| [getDistribution()](#getDistribution--) | Monte Carlo 시뮬레이션에 사용되는 확률 분포를 가져옵니다. |
| [getOptimistic()](#getOptimistic--) | 최적의 프로젝트 시나리오에서 발생할 수 있는 가장 가능성 높은 작업 기간의 비율을 가져옵니다. |
| [getPessimistic()](#getPessimistic--) | 최악의 프로젝트 시나리오에서 발생할 수 있는 가장 가능성 높은 작업 기간의 비율을 가져옵니다. |
| [getTask()](#getTask--) | 이 위험 패턴이 적용되는 프로젝트 작업을 가져옵니다. |
| [setConfidenceLevel(int value)](#setConfidenceLevel-int-) | 실제 생성된 값이 낙관적 및 비관적 추정치 범위 내에 있을 확률 비율에 해당하는 신뢰 수준을 설정합니다. |
| [setDistribution(int value)](#setDistribution-int-) | Monte Carlo 시뮬레이션에 사용되는 확률 분포를 설정합니다. |
| [setOptimistic(int value)](#setOptimistic-int-) | 최적의 프로젝트 시나리오에서 발생할 수 있는 가장 가능성 높은 작업 기간의 비율을 설정합니다. |
| [setPessimistic(int value)](#setPessimistic-int-) | 최악의 프로젝트 시나리오에서 발생할 수 있는 가장 가능성 높은 작업 기간의 비율을 설정합니다. |
### RiskPattern(Task task) {#RiskPattern-com.aspose.tasks.Task-}
```
public RiskPattern(Task task)
```


새 인스턴스를 초기화합니다 [RiskPattern](../../com.aspose.tasks/riskpattern) 클래스.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Monte Carlo 시뮬레이션에서 이 위험이 적용될 지정된 프로젝트 작업. |

### getConfidenceLevel() {#getConfidenceLevel--}
```
public final int getConfidenceLevel()
```


실제 생성된 값이 낙관적 및 비관적 추정치 범위 내에 있을 확률 비율에 해당하는 신뢰 수준을 가져옵니다. 기본값은 CL99입니다.

--------------------

`ConfidenceLevel` 열거형에 정의된 값 중 하나일 수 있습니다 ([getConfidenceLevel()](../../com.aspose.tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose.tasks/riskpattern\#setConfidenceLevel-int-)).

**Returns:**
int - 실제 생성된 값이 낙관적 및 비관적 추정치 범위 내에 있을 확률 비율에 해당하는 신뢰 수준.
### getDistribution() {#getDistribution--}
```
public final int getDistribution()
```


Monte Carlo 시뮬레이션에 사용되는 확률 분포를 가져옵니다. 기본값은 ProbabilityDistributionType.Normal입니다.

--------------------

[ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype) 열거형에 정의된 값 중 하나일 수 있습니다.

**Returns:**
int - Monte Carlo 시뮬레이션에 사용되는 확률 분포.
### getOptimistic() {#getOptimistic--}
```
public final int getOptimistic()
```


최상의 프로젝트 시나리오에서 발생할 수 있는 가장 가능성이 높은 작업 기간의 백분율을 가져옵니다. 기본값은 75이며, 이는 추정된 작업 기간이 4일인 경우 낙관적인 기간이 3일이 됨을 의미합니다.

**Returns:**
int - 최상의 프로젝트 시나리오에서 발생할 수 있는 가장 가능성이 높은 작업 기간의 백분율.
### getPessimistic() {#getPessimistic--}
```
public final int getPessimistic()
```


최악의 프로젝트 시나리오에서 발생할 수 있는 가장 가능성이 높은 작업 기간의 백분율을 가져옵니다. 기본값은 125이며, 이는 추정된 작업 기간이 4일인 경우 비관적인 기간이 5일이 됨을 의미합니다.

**Returns:**
int - 최악의 프로젝트 시나리오에서 발생할 수 있는 가장 가능성이 높은 작업 기간의 백분율.
### getTask() {#getTask--}
```
public final Task getTask()
```


이 위험 패턴이 적용되는 프로젝트 작업을 가져옵니다.

**Returns:**
[Task](../../com.aspose.tasks/task) - a project task to which this risk pattern is applied.
### setConfidenceLevel(int value) {#setConfidenceLevel-int-}
```
public final void setConfidenceLevel(int value)
```


실제 생성된 값이 낙관적 및 비관적 추정치 범위 내에 있을 확률 백분율에 해당하는 신뢰 수준을 설정합니다. 기본값은 CL99입니다.

--------------------

`ConfidenceLevel` 열거형에 정의된 값 중 하나일 수 있습니다 ([getConfidenceLevel()](../../com.aspose.tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose.tasks/riskpattern\#setConfidenceLevel-int-)).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 실제 생성된 값이 낙관적 및 비관적 추정치 범위 내에 있을 확률 백분율에 해당하는 신뢰 수준. |

### setDistribution(int value) {#setDistribution-int-}
```
public final void setDistribution(int value)
```


Monte Carlo 시뮬레이션에 사용되는 확률 분포를 설정합니다. 기본값은 ProbabilityDistributionType.Normal입니다.

--------------------

[ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype) 열거형에 정의된 값 중 하나일 수 있습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | Monte Carlo 시뮬레이션에 사용되는 확률 분포. |

### setOptimistic(int value) {#setOptimistic-int-}
```
public final void setOptimistic(int value)
```


최상의 프로젝트 시나리오에서 발생할 수 있는 가장 가능성이 높은 작업 기간의 백분율을 설정합니다. 기본값은 75이며, 이는 추정된 작업 기간이 4일인 경우 낙관적인 기간이 3일이 됨을 의미합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 최상의 프로젝트 시나리오에서 발생할 수 있는 가장 가능성이 높은 작업 기간의 백분율. |

### setPessimistic(int value) {#setPessimistic-int-}
```
public final void setPessimistic(int value)
```


최악의 프로젝트 시나리오에서 발생할 수 있는 가장 가능성이 높은 작업 기간의 백분율을 설정합니다. 기본값은 125이며, 이는 추정된 작업 기간이 4일인 경우 비관적인 기간이 5일이 됨을 의미합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 최악의 프로젝트 시나리오에서 발생할 수 있는 가장 가능성이 높은 작업 기간의 백분율. |

