---
title: "Task.Set"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Task methode. Koppelt de opgegeven eigenschap aan de opgegeven waarde in deze container"
type: docs
weight: 1410
url: /nl/net/aspose.tasks/task/set/
---
## Task.Set&lt;T&gt; method

Kent de opgegeven eigenschap toe aan de opgegeven waarde in deze container.

```csharp
public void Set<T>(Key<T, TaskKey> key, T val)
```

| Parameter | Beschrijving |
| --- | --- |
| T | het type van de gekoppelde waarde. |
| key | de opgegeven eigenschapssleutel. [`Tsk`](../../tsk/) voor het ophalen van de eigenschapssleutel. |
| waarde | de waarde. |

## Voorbeelden

Toont hoe taakeigenschappen op te halen/instellen.

```csharp
var project = new Project();

// Taak toevoegen en taak‑eigenschappen instellen
var task = project.RootTask.Children.Add();
task.Set(Tsk.Name, "Task1");
task.Set(Tsk.Start, new DateTime(2020, 3, 31, 8, 0, 0));
task.Set(Tsk.Finish, new DateTime(2020, 3, 31, 17, 0, 0));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Alle verzamelde taken doorlopen
foreach (var tsk in collector.Tasks)
{
    Console.WriteLine("Task Id: {0}", tsk.Get(Tsk.Id));
    Console.WriteLine("Task Uid: {0}", tsk.Get(Tsk.Uid));
    Console.WriteLine("Task Name: {0}", tsk.Get(Tsk.Name));
    Console.WriteLine("Task Start: {0}", tsk.Get(Tsk.Start));
    Console.WriteLine("Task Finish: {0}", tsk.Get(Tsk.Finish));
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


