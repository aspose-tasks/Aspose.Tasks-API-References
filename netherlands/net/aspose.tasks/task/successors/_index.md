---
title: "Task.Successors"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Task-eigenschap. Haalt een TaskCollection-object op dat alle opvolgers van dit Task-object bevat"
type: docs
weight: 1200
url: /nl/net/aspose.tasks/task/successors/
---
## Task.Successors property

Haalt een [`TaskCollection`](../../taskcollection/) object op dat alle opvolgers van dit Task-object bevat.

```csharp
public TaskCollection Successors { get; }
```

### Retourwaarde

Alleen-lezen instantie van de [`TaskCollection`](../../taskcollection/) klasse.

## Voorbeelden

Toont hoe de opvolgers van een taak gelezen kunnen worden.

```csharp
var project = new Project();
var pred = project.RootTask.Children.Add("Predecessor");
var succ = project.RootTask.Children.Add("Successor");

project.TaskLinks.Add(pred, succ);

foreach (var successor in pred.Successors)
{
    Console.WriteLine("{0} {1}", successor.Get(Tsk.Id), successor.Get(Tsk.Name));
}
```

### Zie ook

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


