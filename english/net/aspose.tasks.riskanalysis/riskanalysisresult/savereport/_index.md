---
title: RiskAnalysisResult.SaveReport
second_title: Aspose.Tasks for .NET API Reference
description: RiskAnalysisResult method. Saves the risk analysis report to the stream in PDF format
type: docs
weight: 20
url: /net/aspose.tasks.riskanalysis/riskanalysisresult/savereport/
---
## SaveReport(Stream) {#savereport}

Saves the risk analysis report to the stream in PDF format.

```csharp
public void SaveReport(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream to save risk analysis report to. |

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

* class [RiskAnalysisResult](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskanalysisresult/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string) {#savereport_1}

Saves the risk analysis report to the specified file path in PDF format.

```csharp
public void SaveReport(string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The specified file name. |

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

* class [RiskAnalysisResult](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskanalysisresult/)
* assembly [Aspose.Tasks](../../../)


