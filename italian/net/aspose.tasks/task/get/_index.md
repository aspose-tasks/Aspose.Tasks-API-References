---
title: "Task.Get"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Task. Restituisce il valore a cui la proprietà è mappata in questo contenitore"
type: docs
weight: 1340
url: /it/net/aspose.tasks/task/get/
---
## Task.Get&lt;T&gt; method

Restituisce il valore a cui la proprietà è mappata in questo contenitore.

```csharp
public T Get<T>(Key<T, TaskKey> key)
```

| Parametro | Descrizione |
| --- | --- |
| T | il tipo del valore mappato. |
| key | la chiave della proprietà specificata. [`Tsk`](../../tsk/) per ottenere la chiave della proprietà. |

### Valore di ritorno

il valore a cui la proprietà è mappata in questo contenitore.

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


