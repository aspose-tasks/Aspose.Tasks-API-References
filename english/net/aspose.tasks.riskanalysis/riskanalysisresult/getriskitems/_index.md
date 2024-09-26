---
title: RiskAnalysisResult.GetRiskItems
second_title: Aspose.Tasks for .NET API Reference
description: RiskAnalysisResult method. Returns an instance of the RiskItemStatisticsCollection for the specified risk type
type: docs
weight: 10
url: /net/aspose.tasks.riskanalysis/riskanalysisresult/getriskitems/
---
## RiskAnalysisResult.GetRiskItems method

Returns an instance of the [`RiskItemStatisticsCollection`](../../riskitemstatisticscollection/) for the specified risk type.

```csharp
public RiskItemStatisticsCollection GetRiskItems(RiskItemType itemType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| itemType | RiskItemType | the specified risk type; can be one of the values of the [`RiskItemType`](../../riskitemtype/) enumeration. |

### Return Value

an instance of the [`RiskItemStatisticsCollection`](../../riskitemstatisticscollection/) for the specified risk type.

## Examples

Shows how to calculate statistic of risks and save it into as PDF report.

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

// save analysis as a report into a file by file path
analysisResult.SaveReport(OutDir + "AnalysisResult_out.pdf");

// or save analysis into a stream
using (var stream = new FileStream(OutDir + "AnalysisResult_out1.pdf", FileMode.Create))
{
    analysisResult.SaveReport(stream);
}
```

### See Also

* class [RiskItemStatisticsCollection](../../riskitemstatisticscollection/)
* enum [RiskItemType](../../riskitemtype/)
* class [RiskAnalysisResult](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskanalysisresult/)
* assembly [Aspose.Tasks](../../../)


