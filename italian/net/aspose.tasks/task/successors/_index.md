---
title: "Task.Successors"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Task. Ottiene un oggetto TaskCollection che contiene tutti i successori di questo oggetto Task"
type: docs
weight: 1200
url: /it/net/aspose.tasks/task/successors/
---
## Task.Successors property

Ottiene un oggetto [`TaskCollection`](../../taskcollection/) che contiene tutti i successori di questo oggetto Task.

```csharp
public TaskCollection Successors { get; }
```

### Valore di ritorno

Istanza di sola lettura della classe [`TaskCollection`](../../taskcollection/).

## Esempi

Mostra come leggere i successori del task.

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

### Vedi anche

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


