---
title: RiskPattern
second_title: Aspose.Tasks for Python via .NET API Reference
description: 
type: docs
weight: 60
url: /python-net/aspose.tasks.riskanalysis/riskpattern/
---

## RiskPattern class

Represents a risk pattern for a project task.

The RiskPattern type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|RiskPattern(task)|Initializes a new instance of the [RiskPattern](/tasks/python-net/aspose.tasks.riskanalysis/riskpattern/) class.|
## Properties
| Name | Description |
| :- | :- |
|task|Gets a project task to which this risk pattern is applied.|
|distribution|Gets or sets the probability distribution used in Monte Carlo simulation.<br/>            The default value is ProbabilityDistributionType.Normal.|
|confidence_level|Gets or sets the confidence level that correspond to the percentage of the time the actual generated values will be within optimistic and pessimistic estimates.<br/>            The default value is CL99.|
|optimistic|Gets or sets the percentage of the most likely task duration which can happen in the best possible project scenario.<br/>            The default value is 75, which means that if the estimated specified task duration is 4 days then the optimistic duration will be 3 days.|
|pessimistic|Gets or sets the percentage of the most likely task duration which can happen in the worst possible project scenario.<br/>            The default value is 125, which means that if the estimated specified task duration is 4 days then the pessimistic duration will be 5 days.|

### See Also

* namespace [aspose.tasks.riskanalysis](/tasks/python-net/aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](/tasks/python-net/)

