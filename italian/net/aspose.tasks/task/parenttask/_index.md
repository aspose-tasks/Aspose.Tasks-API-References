---
title: "Task.ParentTask"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Task. Ottiene il task genitore di un task"
type: docs
weight: 940
url: /it/net/aspose.tasks/task/parenttask/
---
## Task.ParentTask property

Ottiene l'attività genitore di un'attività.

```csharp
public Task ParentTask { get; }
```

## Esempi

Mostra come utilizzare il task genitore di un task.

```csharp
var project = new Project();
var parent = project.RootTask.Children.Add("Parent");
var child1 = parent.Children.Add("Child1");
var child2 = child1.ParentTask.Children.Add("Child2");

Console.WriteLine("Is parent is equal to the root task: " + child2.ParentTask.Equals(parent));
```

### Vedi anche

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


