---
title: Class RiskItemStatistics
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.RiskAnalysis.RiskItemStatistics class. Represents an item which stores statistical data for the task of the analyzed project
type: docs
weight: 1870
url: /net/aspose.tasks.riskanalysis/riskitemstatistics/
---
## RiskItemStatistics class

Represents an item which stores statistical data for the task of the analyzed project.

```csharp
public class RiskItemStatistics
```

## Properties

| Name | Description |
| --- | --- |
| [ExpectedValue](../../aspose.tasks.riskanalysis/riskitemstatistics/expectedvalue/) { get; } | Gets the expected value of the risk item. |
| [ItemType](../../aspose.tasks.riskanalysis/riskitemstatistics/itemtype/) { get; } | Gets an instance of the [`RiskItemType`](../riskitemtype/) enumeration. |
| [Maximum](../../aspose.tasks.riskanalysis/riskitemstatistics/maximum/) { get; } | Gets the maximum value which was generated during Monte Carlo simulation. |
| [Minimum](../../aspose.tasks.riskanalysis/riskitemstatistics/minimum/) { get; } | Gets the minimum value which was generated during Monte Carlo simulation. |
| [StandardDeviation](../../aspose.tasks.riskanalysis/riskitemstatistics/standarddeviation/) { get; } | Gets the standard deviation of the risk item. |

## Methods

| Name | Description |
| --- | --- |
| [GetPercentile](../../aspose.tasks.riskanalysis/riskitemstatistics/getpercentile/)(int) | Gets a value below which a specified percentage of generated samples fall. |
| override [ToString](../../aspose.tasks.riskanalysis/riskitemstatistics/tostring/)() | Returns short string representation of a risk item. The exact details of the representation are unspecified and subject to change. |

## Examples

Shows how to calculate statistic of risks.

```csharp
var settings = new RiskAnalysisSettings
{
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// Initialize a risk pattern
var pattern = new RiskPattern(task)
{
    // Select a distribution type for the random number generator to generate possible values from (only two types currently supported, namely normal and uniform)            
    // For more details see here: https://en.wikipedia.org/wiki/Normal_distribution)
    Distribution = ProbabilityDistributionType.Normal,

    // Set the percentage of the most likely task duration which can happen in the best possible project scenario 
    // The default value is 75, which means that if the estimated specified task duration is 4 days then the optimistic duration will be 3 days
    Optimistic = 70,

    // Set the percentage of the most likely task duration which can happen in the worst possible project scenario 
    // The default value is 125, which means that if the estimated specified task duration is 4 days then the pessimistic duration will be 5 days.
    Pessimistic = 130,

    // Set a confidence level that correspond to the percentage of the time the actual values will be within optimistic and pessimistic estimates. 
    // You can think of it as a value of standard deviation: the more uncertain about your estimates you are, the more the value of standard deviation used in random number generator is
    ConfidenceLevel = ConfidenceLevel.CL75
};
settings.Patterns.Add(pattern);

// Analyze the project risks
var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);
var statistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Short statistic: " + statistics);
Console.WriteLine();
Console.WriteLine("Statistic details: ");
Console.WriteLine("Item Type: {0}", statistics.ItemType);
Console.WriteLine("Expected value: {0}", statistics.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", statistics.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", statistics.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", statistics.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", statistics.GetPercentile(90));
Console.WriteLine("Minimum: {0}", statistics.Minimum);
Console.WriteLine("Maximum: {0}", statistics.Maximum);
```

### See Also

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


