---
title: "Task.Equals"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Task methode. Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven taak"
type: docs
weight: 1330
url: /nl/net/aspose.tasks/task/equals/
---
## Equals(Task) {#equals}

Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven taak.

```csharp
public bool Equals(Task other)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| anders | Taak | De opgegeven taak om te vergelijken met deze instantie. |

### Retourwaarde

retourneert true als de opgegeven taak en deze instantie gelijke unieke ID's hebben.

## Voorbeelden

Toont hoe je over de toewijzingen van een taak kunt itereren.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // toon de toewijzingen van de taak
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Zie ook

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | Object | Het opgegeven object om te vergelijken met deze instantie. |

### Retourwaarde

retourneert true als de opgegeven taak en deze instantie gelijke unieke ID's hebben.

## Voorbeelden

Toont hoe je over de toewijzingen van een taak kunt itereren.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // toon de toewijzingen van de taak
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Zie ook

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


