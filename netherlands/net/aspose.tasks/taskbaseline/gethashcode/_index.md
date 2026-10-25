---
title: "TaskBaseline.GetHashCode"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskBaseline methode. Retourneert een hashcode‑waarde voor het exemplaar van de TaskBaseline‑klasse"
type: docs
weight: 110
url: /nl/net/aspose.tasks/taskbaseline/gethashcode/
---
## TaskBaseline.GetHashCode method

Retourneert een hashcode‑waarde voor het exemplaar van de [`TaskBaseline`](../) klasse.

```csharp
public override int GetHashCode()
```

### Retourwaarde

retourneert een hashcodewaarde voor dit object.

## Voorbeelden

Toont hoe je de hashcode van een taakbaseline kunt ophalen.

```csharp
var project = new Project();

// TaskBaseline maken
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// taakbaseline-duur weergeven
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// de hashcode van een kalender is gelijk aan het baseline‑nummer
Console.WriteLine("Baseline 1 Number: {0} Hash Code: {1}", (int)baseline1.BaselineNumber, baseline1.GetHashCode());
Console.WriteLine("Baseline 2 Number: {0} Hash Code: {1}", (int)baseline2.BaselineNumber, baseline2.GetHashCode());
```

### Zie ook

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


