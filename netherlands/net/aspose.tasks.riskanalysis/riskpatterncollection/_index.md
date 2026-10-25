---
title: "Klasse RiskPatternCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.RiskAnalysis.RiskPatternCollection class. Vertegenwoordigt een collectie die de instanties van de RiskPattern class bevat."
type: docs
weight: 1940
url: /nl/net/aspose.tasks.riskanalysis/riskpatterncollection/
---
## RiskPatternCollection class

Vertegenwoordigt een collectie die de instanties van de [`RiskPattern`](../riskpattern/) class bevat.

```csharp
public class RiskPatternCollection : ICollection<RiskPattern>, IDictionary<Task, RiskPattern>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks.riskanalysis/riskpatterncollection/count/) { get; } | Haalt het aantal elementen op dat in deze collectie zit. |
| [IsReadOnly](../../aspose.tasks.riskanalysis/riskpatterncollection/isreadonly/) { get; } | Haalt een waarde op die aangeeft of deze collectie alleen-lezen is; anders, false. |
| [Item](../../aspose.tasks.riskanalysis/riskpatterncollection/item/) { get; } | Haalt de instantie van de [`RiskPattern`](../riskpattern/) class op voor de opgegeven taak. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks.riskanalysis/riskpatterncollection/add/)(RiskPattern) | Voegt een instantie van de [`RiskPattern`](../riskpattern/) class toe aan deze collectie. |
| [Clear](../../aspose.tasks.riskanalysis/riskpatterncollection/clear/)() | Verwijdert alle items uit deze collectie. |
| [Contains](../../aspose.tasks.riskanalysis/riskpatterncollection/contains/)(RiskPattern) | Retourneert true als het opgegeven item in deze collectie wordt gevonden; anders false. |
| [CopyTo](../../aspose.tasks.riskanalysis/riskpatterncollection/copyto/)(RiskPattern[], int) | Kopieert de elementen van deze collectie naar de opgegeven array, beginnend bij de opgegeven array-index. |
| [GetEnumerator](../../aspose.tasks.riskanalysis/riskpatterncollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [Remove](../../aspose.tasks.riskanalysis/riskpatterncollection/remove/)(RiskPattern) | Verwijdert de eerste instantie van een specifiek object uit deze collectie. |

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

* class [RiskPattern](../riskpattern/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


