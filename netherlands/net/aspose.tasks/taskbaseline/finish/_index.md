---
title: "TaskBaseline.Finish"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskBaseline eigenschap. Haalt op of stelt de geplande einddatum van de taak in wanneer de baseline is opgeslagen"
type: docs
weight: 40
url: /nl/net/aspose.tasks/taskbaseline/finish/
---
## TaskBaseline.Finish property

Haalt op of stelt de geplande einddatum van de taak in wanneer de basislijn werd opgeslagen.

```csharp
public DateTime Finish { get; set; }
```

## Voorbeelden

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
Console.WriteLine("Baseline duration format: {0}", baseline.Duration.TimeUnit);
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

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


