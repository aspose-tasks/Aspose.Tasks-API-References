---
title: "RiskPattern"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示项目任务的风险模式。"
type: docs
weight: 268
url: /zh/java/com.aspose.tasks/riskpattern/
---

**Inheritance:**
java.lang.Object
```
public class RiskPattern
```

表示项目任务的风险模式。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [RiskPattern(Task task)](#RiskPattern-com.aspose.tasks.Task-) | 初始化 [RiskPattern](../../com.aspose.tasks/riskpattern) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getConfidenceLevel()](#getConfidenceLevel--) | 获取置信水平，该水平对应实际生成值在乐观和悲观估计之间的时间百分比。 |
| [getDistribution()](#getDistribution--) | 获取在蒙特卡罗模拟中使用的概率分布。 |
| [getOptimistic()](#getOptimistic--) | 获取在最佳项目情景下最可能任务持续时间的百分比。 |
| [getPessimistic()](#getPessimistic--) | 获取在最差项目情景下最可能任务持续时间的百分比。 |
| [getTask()](#getTask--) | 获取此风险模式适用的项目任务。 |
| [setConfidenceLevel(int value)](#setConfidenceLevel-int-) | 设置置信水平，该水平对应实际生成值在乐观和悲观估计之间的时间百分比。 |
| [setDistribution(int value)](#setDistribution-int-) | 设置在蒙特卡罗模拟中使用的概率分布。 |
| [setOptimistic(int value)](#setOptimistic-int-) | 设置在最佳项目情景下最可能任务持续时间的百分比。 |
| [setPessimistic(int value)](#setPessimistic-int-) | 设置在最差项目情景下最可能任务持续时间的百分比。 |
### RiskPattern(Task task) {#RiskPattern-com.aspose.tasks.Task-}
```
public RiskPattern(Task task)
```


初始化 [RiskPattern](../../com.aspose.tasks/riskpattern) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 在蒙特卡罗模拟中将此风险应用于的指定项目任务。 |

### getConfidenceLevel() {#getConfidenceLevel--}
```
public final int getConfidenceLevel()
```


获取置信水平，该水平对应实际生成值在乐观和悲观估计之间的时间百分比。默认值为 CL99。

--------------------

可以是 `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose.tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose.tasks/riskpattern\#setConfidenceLevel-int-)) 枚举中定义的值之一。

**Returns:**
int - 对应实际生成值在乐观和悲观估计之间的时间百分比的置信水平。
### getDistribution() {#getDistribution--}
```
public final int getDistribution()
```


获取在 Monte Carlo 仿真中使用的概率分布。默认值为 ProbabilityDistributionType.Normal。

--------------------

可以是 [ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype) 枚举中定义的值之一。

**Returns:**
int - 在 Monte Carlo 仿真中使用的概率分布。
### getOptimistic() {#getOptimistic--}
```
public final int getOptimistic()
```


获取在最佳项目情景下可能出现的最可能任务持续时间的百分比。默认值为 75，这意味着如果估计的任务持续时间为 4 天，则乐观持续时间为 3 天。

**Returns:**
int - 在最佳项目情景下可能出现的最可能任务持续时间的百分比。
### getPessimistic() {#getPessimistic--}
```
public final int getPessimistic()
```


获取在最差项目情景下可能出现的最可能任务持续时间的百分比。默认值为 125，这意味着如果估计的任务持续时间为 4 天，则悲观持续时间为 5 天。

**Returns:**
int - 在最差项目情景下可能出现的最可能任务持续时间的百分比。
### getTask() {#getTask--}
```
public final Task getTask()
```


获取此风险模式适用的项目任务。

**Returns:**
[Task](../../com.aspose.tasks/task) - a project task to which this risk pattern is applied.
### setConfidenceLevel(int value) {#setConfidenceLevel-int-}
```
public final void setConfidenceLevel(int value)
```


设置对应于实际生成值在乐观和悲观估计范围内出现的时间百分比的置信水平。默认值为 CL99。

--------------------

可以是 `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose.tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose.tasks/riskpattern\#setConfidenceLevel-int-)) 枚举中定义的值之一。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 对应于实际生成值在乐观和悲观估计范围内出现的时间百分比的置信水平。 |

### setDistribution(int value) {#setDistribution-int-}
```
public final void setDistribution(int value)
```


设置在 Monte Carlo 仿真中使用的概率分布。默认值为 ProbabilityDistributionType.Normal。

--------------------

可以是 [ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype) 枚举中定义的值之一。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 在 Monte Carlo 仿真中使用的概率分布。 |

### setOptimistic(int value) {#setOptimistic-int-}
```
public final void setOptimistic(int value)
```


设置在最佳项目情景下可能出现的最可能任务持续时间的百分比。默认值为 75，这意味着如果估计的任务持续时间为 4 天，则乐观持续时间为 3 天。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 在最佳项目情景下可能出现的最可能任务持续时间的百分比。 |

### setPessimistic(int value) {#setPessimistic-int-}
```
public final void setPessimistic(int value)
```


设置在最差项目情景下可能出现的最可能任务持续时间的百分比。默认值为 125，这意味着如果估计的任务持续时间为 4 天，则悲观持续时间为 5 天。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 在最差项目情景下可能出现的最可能任务持续时间的百分比。 |

