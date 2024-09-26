---
title: RiskPatternCollection.Item
second_title: Aspose.Tasks for .NET API Reference
description: RiskPatternCollection property. Gets the instance of the RiskPattern class for the specified task
type: docs
weight: 30
url: /net/aspose.tasks.riskanalysis/riskpatterncollection/item/
---
## RiskPatternCollection indexer

Gets the instance of the [`RiskPattern`](../../riskpattern/) class for the specified task.

```csharp
public RiskPattern this[Task task] { get; }
```

| Parameter | Description |
| --- | --- |
| task | the specified task. |

### Return Value

the pattern for the specified task.

## Examples

Shows how to work with risk pattern collections.

```csharp
var settings = new RiskAnalysisSettings
{
    // Set number of iterations for Monte Carlo simulation (the default value is 100).
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task1 = project.RootTask.Children.GetById(17);
var task2 = project.RootTask.Children.GetById(18);

// as far as RiskPatternCollection is not a read-only
Console.WriteLine("Is pattern collection read-only?: " + settings.Patterns.IsReadOnly);

// one can add new patterns 
var pattern1 = new RiskPattern(task1)
{
    Distribution = ProbabilityDistributionType.Normal,
    Optimistic = 60,
    Pessimistic = 140,
    ConfidenceLevel = ConfidenceLevel.CL75
};
var pattern2 = new RiskPattern(task2)
{
    Distribution = ProbabilityDistributionType.Normal,
    Optimistic = 70,
    Pessimistic = 130,
    ConfidenceLevel = ConfidenceLevel.CL75
};

settings.Patterns.Add(pattern1);
settings.Patterns.Add(pattern2);

// iterate over added patterns
Console.WriteLine("Patterns count: " + settings.Patterns.Count);
foreach (var pattern in settings.Patterns)
{
    Console.WriteLine("Task: " + pattern.Task);
    Console.WriteLine("Distribution: " + pattern.Distribution);
    Console.WriteLine("Optimistic: " + pattern.Optimistic);
    Console.WriteLine("Pessimistic: " + pattern.Pessimistic);
    Console.WriteLine("Confidence Level: " + pattern.ConfidenceLevel);
    Console.WriteLine();
}

// edit the pattern in the collection by using index access
settings.Patterns[task1].Optimistic = 70;
settings.Patterns[task1].Pessimistic = 140;

// check patterns after edits
Console.WriteLine("Print edited patterns: ");
foreach (var pattern in settings.Patterns)
{
    Console.WriteLine("Task: " + pattern.Task);
    Console.WriteLine("Distribution: " + pattern.Distribution);
    Console.WriteLine("Optimistic: " + pattern.Optimistic);
    Console.WriteLine("Pessimistic: " + pattern.Pessimistic);
    Console.WriteLine("Confidence Level: " + pattern.ConfidenceLevel);
    Console.WriteLine();
}

// we can remove the pattern
Console.WriteLine("Removing the first pattern...");
settings.Patterns.Remove(pattern1);

// check that pattern not in the collection
Console.WriteLine("Is collection contains the first pattern?: " + settings.Patterns.Contains(pattern1));

// one can clear the collection in two ways

// copy patterns into the array and delete them one by one
var patterns = new RiskPattern[settings.Patterns.Count];
settings.Patterns.CopyTo(patterns, 0);
foreach (var pattern in patterns)
{
    settings.Patterns.Remove(pattern);
}

// or one can clear a pattern collection completely
settings.Patterns.Clear();
```

### See Also

* class [RiskPattern](../../riskpattern/)
* class [Task](../../../aspose.tasks/task/)
* class [RiskPatternCollection](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskpatterncollection/)
* assembly [Aspose.Tasks](../../../)


