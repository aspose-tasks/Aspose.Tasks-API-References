---
title: "Task.Predecessors"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Task. Ottiene un oggetto TaskCollection che contiene tutti i predecessori di questo oggetto Task"
type: docs
weight: 980
url: /it/net/aspose.tasks/task/predecessors/
---
## Task.Predecessors property

Ottiene un oggetto [`TaskCollection`](../../taskcollection/) che contiene tutti i predecessori di questo oggetto Task.

```csharp
public TaskCollection Predecessors { get; }
```

### Valore di ritorno

Istanza di sola lettura della classe [`TaskCollection`](../../taskcollection/).

## Esempi

Mostra come leggere i predecessori dell'attività.

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

### Vedi anche

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


