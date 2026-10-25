---
title: "DurationFormat"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Haalt het formaat op of stelt het in voor het weergeven van de duur van de taakbaseline."
type: docs
weight: 30
url: /nl/net/aspose.tasks/taskbaseline/durationformat/
---
## TaskBaseline.DurationFormat property

Haalt het formaat op of stelt het in voor het weergeven van de duur van de taakbaseline.

```csharp
public TimeUnitType DurationFormat { get; set; }
```

### Voorbeelden

Toont hoe toegang te krijgen tot basislijninformatie.

```csharp
var project = new Project();

// TaskBaseline aanmaken
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Taakbasislangeduur weergeven
var baseline = task.Baselines.ToList()[0];
Console.WriteLine("Baseline Start: {0}", baseline.Start);
Console.WriteLine("Baseline duration: {0}", baseline.Duration);
Console.WriteLine("Baseline duration format: {0}", baseline.DurationFormat);
Console.WriteLine("Is it estimated duration?: {0}", baseline.EstimatedDuration);
Console.WriteLine("Baseline Finish: {0}", baseline.Finish);

// waarde die aangeeft of dit een tussentijdse basislijn is
Console.WriteLine("Interim: {0}", baseline.Interim);
Console.WriteLine("Fixed Cost: {0}", baseline.FixedCost);

// tijdgephaseerde gegevens van taakbasislijn afdrukken
Console.WriteLine("Number of timephased items: " + baseline.TimephasedData.Count);
foreach (var data in baseline.TimephasedData)
{
    Console.WriteLine(" Uid: " + data.Uid);
    Console.WriteLine(" Start: " + data.Start);
    Console.WriteLine(" Finish: " + data.Finish);
}
```

### Zie ook

* enum [TimeUnitType](../../timeunittype)
* class [TaskBaseline](../../taskbaseline)
* namespace [Aspose.Tasks](../../taskbaseline)
* assembly [Aspose.Tasks](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor Aspose.Tasks.dll -->
