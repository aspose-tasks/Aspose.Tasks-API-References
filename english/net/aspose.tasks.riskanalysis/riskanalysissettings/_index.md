---
title: Class RiskAnalysisSettings
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.RiskAnalysis.RiskAnalysisSettings class. Specifies settings for performing risk analysis
type: docs
weight: 1820
url: /net/aspose.tasks.riskanalysis/riskanalysissettings/
---
## RiskAnalysisSettings class

Specifies settings for performing risk analysis.

```csharp
public class RiskAnalysisSettings
```

## Constructors

| Name | Description |
| --- | --- |
| [RiskAnalysisSettings](riskanalysissettings/)() | Initializes a new instance of the `RiskAnalysisSettings` class. |

## Properties

| Name | Description |
| --- | --- |
| [IterationsCount](../../aspose.tasks.riskanalysis/riskanalysissettings/iterationscount/) { get; set; } | Gets or sets the number of iterations to use in Monte Carlo simulation. The default value is 100. |
| [Patterns](../../aspose.tasks.riskanalysis/riskanalysissettings/patterns/) { get; } | Gets a collection containing the instances of the [`RiskPattern`](../riskpattern/) class. |

## Examples

Shows how to prepare risk analysis settings for Monte-Carlo simulations.

```csharp
var riskAnalysisSettings = new RiskAnalysisSettings();

// Set number of iterations for Monte Carlo simulation (the default value is 100).
riskAnalysisSettings.IterationsCount = 200;

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

riskAnalysisSettings.Patterns.Add(pattern);

var analyzer = new RiskAnalyzer(riskAnalysisSettings);
var analysisResult = analyzer.Analyze(project);
var rootEarlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", rootEarlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", rootEarlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", rootEarlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", rootEarlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", rootEarlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", rootEarlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", rootEarlyFinish.Maximum);

analysisResult.SaveReport(OutDir + "AnalysisReport_out.pdf");
```

### See Also

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


