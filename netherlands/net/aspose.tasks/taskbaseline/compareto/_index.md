---
title: "TaskBaseline.CompareTo"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskBaseline methode. IComparable interface-implementatie. Vergelijkt dit exemplaar met het opgegeven Baseline-object"
type: docs
weight: 90
url: /nl/net/aspose.tasks/taskbaseline/compareto/
---
## TaskBaseline.CompareTo method

IComparable‑interface‑implementatie. Vergelijkt deze instantie met het opgegeven Baseline‑object.

```csharp
public int CompareTo(TaskBaseline other)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| anders | TaskBaseline | het opgegeven Baseline‑object waarmee deze instantie wordt vergeleken. |

### Retourwaarde

returnt -1 als deze instantie kleiner is dan het opgegeven object, 1 als deze instantie groter is dan het opgegeven object; anders returnt het 0

## Voorbeelden

Toont hoe de gelijkheid van baselines te controleren.

```csharp
var project = new Project();

// TaskBaseline maken
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// taakbaseline-duur weergeven
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// de gelijkheid van baselines wordt gecontroleerd aan de hand van de cijfers van de baseline.
Console.WriteLine("Baseline Number 1: " + baseline1.BaselineNumber);
Console.WriteLine("Baseline Number 2: " + baseline2.BaselineNumber);
Console.WriteLine("Are baselines equal: " + baseline1.Equals(baseline2));
```

### Zie ook

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


