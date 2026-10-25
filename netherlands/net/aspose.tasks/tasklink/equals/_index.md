---
title: "TaskLink.Equals"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskLink methode. Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object"
type: docs
weight: 90
url: /nl/net/aspose.tasks/tasklink/equals/
---
## Equals(TaskLink) {#equals}

Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

```csharp
public bool Equals(TaskLink other)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | TaskLink | De opgegeven instantie van de [`TaskLink`](../) klasse om te vergelijken met deze instantie. |

### Retourwaarde

**True** if the specified instance of the [`TaskLink`](../) class has the same predecessor and successor tasks as this instance; otherwise, **false**.

## Voorbeelden

Toont hoe de gelijkheid van taakkoppelingen te controleren.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// De gelijkheid van taakkoppelingen is gebaseerd op voorganger- en opvolgertaken.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### Zie ook

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | Object | Het object om te vergelijken met deze instantie. |

### Retourwaarde

**True** if the specified object is a TaskLink that has the same predecessor and successor as this instance; otherwise, **false**.

## Voorbeelden

Toont hoe de gelijkheid van taakkoppelingen te controleren.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// De gelijkheid van taakkoppelingen is gebaseerd op voorganger- en opvolgertaken.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### Zie ook

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


