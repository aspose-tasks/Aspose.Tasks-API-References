---
title: "Task.Set"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Task. Mappa la proprietà specificata al valore specificato in questo contenitore"
type: docs
weight: 1410
url: /it/net/aspose.tasks/task/set/
---
## Task.Set&lt;T&gt; method

Mappa la proprietà specificata al valore specificato in questo contenitore.

```csharp
public void Set<T>(Key<T, TaskKey> key, T val)
```

| Parametro | Descrizione |
| --- | --- |
| T | il tipo del valore mappato. |
| key | la chiave della proprietà specificata. [`Tsk`](../../tsk/) per ottenere la chiave della proprietà. |
| val | il valore. |

## Esempi

Mostra come ottenere/impostare le proprietà del task.

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
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


