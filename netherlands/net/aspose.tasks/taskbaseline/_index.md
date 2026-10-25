---
title: "Klasse TaskBaseline"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.TaskBaseline klasse. Vertegenwoordigt de baseline van een taak"
type: docs
weight: 2370
url: /nl/net/aspose.tasks/taskbaseline/
---
## TaskBaseline class

Stelt de basislijn van een taak voor.

```csharp
public sealed class TaskBaseline : Baseline, IComparable<TaskBaseline>, IEquatable<TaskBaseline>
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [TaskBaseline](taskbaseline/)(Task) | Initialiseert een nieuw exemplaar van de `TaskBaseline`-klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Haalt op of stelt het unieke nummer van een baseline-gegevensrecord in. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Haalt op of stelt de begrote kosten van een door een resource uitgevoerd werk voor een project tot nu toe in. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Haalt op of stelt de budgetkosten van een voor een resource gepland werk in. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Haalt op of stelt de geprojecteerde kosten van een resource in wanneer de baseline wordt opgeslagen. |
| [Duration](../../aspose.tasks/taskbaseline/duration/) { get; set; } | Haalt op of stelt de geplande duur van de taak in wanneer de basislijn werd opgeslagen. |
| [EstimatedDuration](../../aspose.tasks/taskbaseline/estimatedduration/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de basislangeduur van de taak werd geschat. |
| [Finish](../../aspose.tasks/taskbaseline/finish/) { get; set; } | Haalt op of stelt de geplande einddatum van de taak in wanneer de basislijn werd opgeslagen. |
| [FixedCost](../../aspose.tasks/taskbaseline/fixedcost/) { get; set; } | Haalt op of stelt een vaste kostprijs van de taak in wanneer de basislijn werd opgeslagen. |
| [Interim](../../aspose.tasks/taskbaseline/interim/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of dit een tussentijdse basislijn is. |
| [Start](../../aspose.tasks/taskbaseline/start/) { get; set; } | Haalt op of stelt de geplande startdatum van de taak in wanneer de basislijn werd opgeslagen. |
| [TimephasedData](../../aspose.tasks/taskbaseline/timephaseddata/) { get; set; } | Haalt op of stelt een `TimephasedDataCollection`-instantie voor dit object in. De tijdgephaseerde gegevens die aan de taakbasislijn zijn gekoppeld. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Haalt op of stelt het werk in dat aan een resource is toegewezen wanneer de baseline wordt opgeslagen. De hoeveelheid toegewezen werk aan een resource wanneer de baseline werd opgeslagen. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | IComparable‑interface‑implementatie. Vergelijkt deze instantie met het opgegeven Baseline‑object. |
| [CompareTo](../../aspose.tasks/taskbaseline/compareto/#compareto_1)(TaskBaseline) | IComparable‑interface‑implementatie. Vergelijkt deze instantie met het opgegeven Baseline‑object. |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| override [Equals](../../aspose.tasks/taskbaseline/equals/#equals_2)(object) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [Equals](../../aspose.tasks/taskbaseline/equals/#equals_1)(TaskBaseline) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven TaskBaseline‑object. |
| override [GetHashCode](../../aspose.tasks/taskbaseline/gethashcode/)() | Retourneert een hashcode‑waarde voor de instantie van de `TaskBaseline`‑klasse. |

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

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


