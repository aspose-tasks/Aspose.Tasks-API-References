---
title: Class RiskItemStatisticsCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.RiskAnalysis.RiskItemStatisticsCollection class. Represents a collection containing the instances of the RiskItemStatistics class
type: docs
weight: 1880
url: /net/aspose.tasks.riskanalysis/riskitemstatisticscollection/
---
## RiskItemStatisticsCollection class

Represents a collection containing the instances of the [`RiskItemStatistics`](../riskitemstatistics/) class.

```csharp
public class RiskItemStatisticsCollection : IDictionary<Task, RiskItemStatistics>, 
    IEnumerable<RiskItemStatistics>
```

## Methods

| Name | Description |
| --- | --- |
| [Get](../../aspose.tasks.riskanalysis/riskitemstatisticscollection/get/)(Task) | Returns an instance of the [`RiskItemStatistics`](../riskitemstatistics/) class containing in this collection which is associated with the specified Task object; null if the item is not found. |
| [GetEnumerator](../../aspose.tasks.riskanalysis/riskitemstatisticscollection/getenumerator/)() | Returns an enumerator for this collection. |

## Examples

Shows how to work with collection of risk statistics.

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

var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);

// iterate over all statistic items
var statistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish);

foreach (var statistic in statistics)
{
    Console.WriteLine("Short statistic: " + statistic);
    Console.WriteLine();
    Console.WriteLine("Statistic details: ");
    Console.WriteLine("Item Type: {0}", statistic.ItemType);
    Console.WriteLine("Expected value: {0}", statistic.ExpectedValue);
    Console.WriteLine("StandardDeviation: {0}", statistic.StandardDeviation);
    Console.WriteLine("10% Percentile: {0}", statistic.GetPercentile(10));
    Console.WriteLine("50% Percentile: {0}", statistic.GetPercentile(50));
    Console.WriteLine("90% Percentile: {0}", statistic.GetPercentile(90));
    Console.WriteLine("Minimum: {0}", statistic.Minimum);
    Console.WriteLine("Maximum: {0}", statistic.Maximum);
}

// or get a specific stats
var itemStatistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Print the specific statistic: ");
Console.WriteLine("Expected value: {0}", itemStatistics.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", itemStatistics.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", itemStatistics.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", itemStatistics.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", itemStatistics.GetPercentile(90));
Console.WriteLine("Minimum: {0}", itemStatistics.Minimum);
Console.WriteLine("Maximum: {0}", itemStatistics.Maximum);
```

### See Also

* class [Task](../../aspose.tasks/task/)
* class [RiskItemStatistics](../riskitemstatistics/)
* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


