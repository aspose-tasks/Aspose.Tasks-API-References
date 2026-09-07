---
title: "Task.SelectAllChildTasks"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Task. Raccoglie ricorsivamente tutti i task figli di questo task"
type: docs
weight: 1400
url: /it/net/aspose.tasks/task/selectallchildtasks/
---
## Task.SelectAllChildTasks method

Raccoglie ricorsivamente tutte le attività figlie di questa attività.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### Valore di ritorno

Un elenco di task figli di questo task.

## Esempi

Mostra come iterare sui task figli.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task 1");
task.Children.Add("Task 2");

foreach (var tsk in project.RootTask.SelectAllChildTasks())
{
    Console.WriteLine("{0} {1}", tsk.Get(Tsk.Id), tsk.Get(Tsk.Name));
}
```

### Vedi anche

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


