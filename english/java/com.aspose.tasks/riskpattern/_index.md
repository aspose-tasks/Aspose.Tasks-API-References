---
title: RiskPattern
second_title: Aspose.Tasks for Java API Reference
description: Represents a risk pattern for a project task.
type: docs
weight: 267
url: /java/com.aspose.tasks/riskpattern/
---

**Inheritance:**
java.lang.Object
```
public class RiskPattern
```

Represents a risk pattern for a project task.
## Constructors

| Constructor | Description |
| --- | --- |
| [RiskPattern(Task task)](#RiskPattern-com.aspose.tasks.Task-) | Initializes a new instance of the [RiskPattern](../../com.aspose.tasks/riskpattern) class. |
## Methods

| Method | Description |
| --- | --- |
| [getConfidenceLevel()](#getConfidenceLevel--) | Gets the confidence level that correspond to the percentage of the time the actual generated values will be within optimistic and pessimistic estimates. |
| [getDistribution()](#getDistribution--) | Gets the probability distribution used in Monte Carlo simulation. |
| [getOptimistic()](#getOptimistic--) | Gets the percentage of the most likely task duration which can happen in the best possible project scenario. |
| [getPessimistic()](#getPessimistic--) | Gets the percentage of the most likely task duration which can happen in the worst possible project scenario. |
| [getTask()](#getTask--) | Gets a project task to which this risk pattern is applied. |
| [setConfidenceLevel(int value)](#setConfidenceLevel-int-) | Sets the confidence level that correspond to the percentage of the time the actual generated values will be within optimistic and pessimistic estimates. |
| [setDistribution(int value)](#setDistribution-int-) | Sets the probability distribution used in Monte Carlo simulation. |
| [setOptimistic(int value)](#setOptimistic-int-) | Sets the percentage of the most likely task duration which can happen in the best possible project scenario. |
| [setPessimistic(int value)](#setPessimistic-int-) | Sets the percentage of the most likely task duration which can happen in the worst possible project scenario. |
### RiskPattern(Task task) {#RiskPattern-com.aspose.tasks.Task-}
```
public RiskPattern(Task task)
```


Initializes a new instance of the [RiskPattern](../../com.aspose.tasks/riskpattern) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | the specified project task for which this risk will be applied in Monte Carlo simulation. |

### getConfidenceLevel() {#getConfidenceLevel--}
```
public final int getConfidenceLevel()
```


Gets the confidence level that correspond to the percentage of the time the actual generated values will be within optimistic and pessimistic estimates. The default value is CL99.

--------------------

Can be one of the values defined in the `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose.tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose.tasks/riskpattern\#setConfidenceLevel-int-)) enumeration.

**Returns:**
int - the confidence level that correspond to the percentage of the time the actual generated values will be within optimistic and pessimistic estimates.
### getDistribution() {#getDistribution--}
```
public final int getDistribution()
```


Gets the probability distribution used in Monte Carlo simulation. The default value is ProbabilityDistributionType.Normal.

--------------------

Can be one of the values defined in the [ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype) enumeration.

**Returns:**
int - the probability distribution used in Monte Carlo simulation.
### getOptimistic() {#getOptimistic--}
```
public final int getOptimistic()
```


Gets the percentage of the most likely task duration which can happen in the best possible project scenario. The default value is 75, which means that if the estimated specified task duration is 4 days then the optimistic duration will be 3 days.

**Returns:**
int - the percentage of the most likely task duration which can happen in the best possible project scenario.
### getPessimistic() {#getPessimistic--}
```
public final int getPessimistic()
```


Gets the percentage of the most likely task duration which can happen in the worst possible project scenario. The default value is 125, which means that if the estimated specified task duration is 4 days then the pessimistic duration will be 5 days.

**Returns:**
int - the percentage of the most likely task duration which can happen in the worst possible project scenario.
### getTask() {#getTask--}
```
public final Task getTask()
```


Gets a project task to which this risk pattern is applied.

**Returns:**
[Task](../../com.aspose.tasks/task) - a project task to which this risk pattern is applied.
### setConfidenceLevel(int value) {#setConfidenceLevel-int-}
```
public final void setConfidenceLevel(int value)
```


Sets the confidence level that correspond to the percentage of the time the actual generated values will be within optimistic and pessimistic estimates. The default value is CL99.

--------------------

Can be one of the values defined in the `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose.tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose.tasks/riskpattern\#setConfidenceLevel-int-)) enumeration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the confidence level that correspond to the percentage of the time the actual generated values will be within optimistic and pessimistic estimates. |

### setDistribution(int value) {#setDistribution-int-}
```
public final void setDistribution(int value)
```


Sets the probability distribution used in Monte Carlo simulation. The default value is ProbabilityDistributionType.Normal.

--------------------

Can be one of the values defined in the [ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype) enumeration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the probability distribution used in Monte Carlo simulation. |

### setOptimistic(int value) {#setOptimistic-int-}
```
public final void setOptimistic(int value)
```


Sets the percentage of the most likely task duration which can happen in the best possible project scenario. The default value is 75, which means that if the estimated specified task duration is 4 days then the optimistic duration will be 3 days.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the percentage of the most likely task duration which can happen in the best possible project scenario. |

### setPessimistic(int value) {#setPessimistic-int-}
```
public final void setPessimistic(int value)
```


Sets the percentage of the most likely task duration which can happen in the worst possible project scenario. The default value is 125, which means that if the estimated specified task duration is 4 days then the pessimistic duration will be 5 days.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the percentage of the most likely task duration which can happen in the worst possible project scenario. |

