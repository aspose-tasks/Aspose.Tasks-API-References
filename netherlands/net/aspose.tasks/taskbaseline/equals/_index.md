---
title: "TaskBaseline.Equals"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskBaseline methode. Retourneert een waarde die aangeeft of dit exemplaar gelijk is aan het opgegeven TaskBaseline‑object"
type: docs
weight: 100
url: /nl/net/aspose.tasks/taskbaseline/equals/
---
## Equals(TaskBaseline) {#equals_1}

Retourneert een waarde die aangeeft of deze instantie gelijk is aan het opgegeven TaskBaseline‑object.

```csharp
public bool Equals(TaskBaseline other)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| anders | TaskBaseline | het opgegeven AssignmentBaseline-object om te vergelijken met deze instantie. |

### Retourwaarde

retourneert true als dit exemplaar gelijk is aan het opgegeven TaskBaseline‑object; anders false.

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

---

## Equals(object) {#equals_2}

Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | Object | Het object om te vergelijken met deze instantie. |

### Retourwaarde

**True** if the specified object is a TaskBaseline that has the same UID value as this instance; otherwise, **false**.

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


