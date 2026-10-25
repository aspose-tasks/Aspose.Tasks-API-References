---
title: "Tsk.Uid"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. L'ID univoco di un'attività"
type: docs
weight: 1110
url: /it/net/aspose.tasks/tsk/uid/
---
## Tsk.Uid field

L'Id univoco di un'attività.

```csharp
public static readonly Key<int, TaskKey> Uid;
```

## Esempi

Mostra come leggere/scrivere le proprietà del task.

```csharp
var project = new Project();

// Aggiungi un task e imposta le proprietà del task
var task = project.RootTask.Children.Add();
task.Set(Tsk.Name, "Task1");
task.Set(Tsk.Start, new DateTime(2020, 3, 31, 8, 0, 0));
task.Set(Tsk.Finish, new DateTime(2020, 3, 31, 17, 0, 0));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analizza tutti i task raccolti
foreach (var tsk in collector.Tasks)
{
    Console.WriteLine("Task Id: {0}", tsk.Get(Tsk.Id));
    Console.WriteLine("Task Uid: {0}", tsk.Get(Tsk.Uid));
    Console.WriteLine("Task Name: {0}", tsk.Get(Tsk.Name));
    Console.WriteLine("Task Start: {0}", tsk.Get(Tsk.Start));
    Console.WriteLine("Task Finish: {0}", tsk.Get(Tsk.Finish));
}
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


