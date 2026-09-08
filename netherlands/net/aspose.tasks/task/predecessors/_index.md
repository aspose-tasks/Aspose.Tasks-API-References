---
title: "Task.Predecessors"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Task eigenschap. Haalt een TaskCollection object op dat alle voorgangers van dit Task object bevat"
type: docs
weight: 980
url: /nl/net/aspose.tasks/task/predecessors/
---
## Task.Predecessors property

Haalt een [`TaskCollection`](../../taskcollection/) object op dat alle voorgangers van dit Task object bevat.

```csharp
public TaskCollection Predecessors { get; }
```

### Retourwaarde

Alleen-lezen instantie van de [`TaskCollection`](../../taskcollection/) klasse.

## Voorbeelden

Toont hoe de voorgangers van een taak gelezen worden.

```csharp
var project = new Project();
var pred = project.RootTask.Children.Add("Predecessor");
var succ = project.RootTask.Children.Add("Successor");

project.TaskLinks.Add(pred, succ);

foreach (var predecessor in succ.Predecessors)
{
    Console.WriteLine("{0} {1}", predecessor.Get(Tsk.Id), predecessor.Get(Tsk.Name));
}
```

### Zie ook

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


