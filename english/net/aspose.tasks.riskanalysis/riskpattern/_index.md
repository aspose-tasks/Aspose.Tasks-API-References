---
title: Class RiskPattern
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.RiskAnalysis.RiskPattern class. Represents a risk pattern for a project task
type: docs
weight: 1860
url: /net/aspose.tasks.riskanalysis/riskpattern/
---
## RiskPattern class

Represents a risk pattern for a project task.

```csharp
public class RiskPattern
```

## Constructors

| Name | Description |
| --- | --- |
| [RiskPattern](riskpattern/)(Task) | Initializes a new instance of the `RiskPattern` class. |

## Properties

| Name | Description |
| --- | --- |
| [ConfidenceLevel](../../aspose.tasks.riskanalysis/riskpattern/confidencelevel/) { get; set; } | Gets or sets the confidence level that correspond to the percentage of the time the actual generated values will be within optimistic and pessimistic estimates. The default value is CL99. |
| [Distribution](../../aspose.tasks.riskanalysis/riskpattern/distribution/) { get; set; } | Gets or sets the probability distribution used in Monte Carlo simulation. The default value is ProbabilityDistributionType.Normal. |
| [Optimistic](../../aspose.tasks.riskanalysis/riskpattern/optimistic/) { get; set; } | Gets or sets the percentage of the most likely task duration which can happen in the best possible project scenario. The default value is 75, which means that if the estimated specified task duration is 4 days then the optimistic duration will be 3 days. |
| [Pessimistic](../../aspose.tasks.riskanalysis/riskpattern/pessimistic/) { get; set; } | Gets or sets the percentage of the most likely task duration which can happen in the worst possible project scenario. The default value is 125, which means that if the estimated specified task duration is 4 days then the pessimistic duration will be 5 days. |
| [Task](../../aspose.tasks.riskanalysis/riskpattern/task/) { get; } | Gets a project task to which this risk pattern is applied. |

## Examples

Shows how to define risk simulation settings.

```csharp
var settings = new RiskAnalysisSettings();
settings.IterationsCount = 200;

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// Initialize a risk pattern
var pattern = new RiskPattern(task);

// Select a distribution type for the random number generator to generate possible values from (only two types currently supported, namely normal and uniform)            
// For more details see here: https://en.wikipedia.org/wiki/Normal_distribution)
pattern.Distribution = ProbabilityDistributionType.Normal;

// Set the percentage of the most likely task duration which can happen in the best possible project scenario 
// The default value is 75, which means that if the estimated specified task duration is 4 days then the optimistic duration will be 3 days
pattern.Optimistic = 70;

// Set the percentage of the most likely task duration which can happen in the worst possible project scenario 
// The default value is 125, which means that if the estimated specified task duration is 4 days then the pessimistic duration will be 5 days.
pattern.Pessimistic = 130;

// Set a confidence level that correspond to the percentage of the time the actual values will be within optimistic and pessimistic estimates. 
// You can think of it as a value of standard deviation: the more uncertain about your estimates you are, the more the value of standard deviation used in random number generator is
pattern.ConfidenceLevel = ConfidenceLevel.CL75;

settings.Patterns.Add(pattern);

var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);
var earlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", earlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", earlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", earlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", earlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", earlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", earlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", earlyFinish.Maximum);

analysisResult.SaveReport(OutDir + "AnalysisReport_out.pdf");
```

### See Also

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


