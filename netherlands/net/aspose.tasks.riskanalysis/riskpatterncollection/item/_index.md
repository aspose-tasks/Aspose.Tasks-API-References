---
title: "RiskPatternCollection.Item"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "RiskPatternCollection eigenschap. Haalt de instantie van de RiskPattern-klasse op voor de opgegeven taak"
type: docs
weight: 30
url: /nl/net/aspose.tasks.riskanalysis/riskpatterncollection/item/
---
## RiskPatternCollection indexer

Haalt de instantie van de [`RiskPattern`](../../riskpattern/) klasse op voor de opgegeven taak.

```csharp
public RiskPattern this[Task task] { get; }
```

| Parameter | Beschrijving |
| --- | --- |
| taak | de opgegeven taak. |

### Retourwaarde

het patroon voor de opgegeven taak.

## Voorbeelden

Toont hoe te werken met risicopatrooncollecties.

```csharp
var settings = new RiskAnalysisSettings
{
    // Stel het aantal iteraties in voor Monte Carlo-simulatie (de standaardwaarde is 100).
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task1 = project.RootTask.Children.GetById(17);
var task2 = project.RootTask.Children.GetById(18);

// aangezien RiskPatternCollection niet alleen-lezen is
Console.WriteLine("Is pattern collection read-only?: " + settings.Patterns.IsReadOnly);

// kan nieuwe patronen toevoegen 
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

// itereren over toegevoegde patronen
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

// bewerk het patroon in de collectie door indextoegang te gebruiken
settings.Patterns[task1].Optimistic = 70;
settings.Patterns[task1].Pessimistic = 140;

// controleer patronen na bewerkingen
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

// we kunnen het patroon verwijderen
Console.WriteLine("Removing the first pattern...");
settings.Patterns.Remove(pattern1);

// controleer dat het patroon niet in de collectie zit
Console.WriteLine("Is collection contains the first pattern?: " + settings.Patterns.Contains(pattern1));

// men kan de collectie op twee manieren wissen

// kopieer patronen naar de array en verwijder ze één voor één
var patterns = new RiskPattern[settings.Patterns.Count];
settings.Patterns.CopyTo(patterns, 0);
foreach (var pattern in patterns)
{
    settings.Patterns.Remove(pattern);
}

// of men kan een patrooncollectie volledig wissen
settings.Patterns.Clear();
```

### Zie ook

* class [RiskPattern](../../riskpattern/)
* class [Task](../../../aspose.tasks/task/)
* class [RiskPatternCollection](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskpatterncollection/)
* assembly [Aspose.Tasks](../../../)


