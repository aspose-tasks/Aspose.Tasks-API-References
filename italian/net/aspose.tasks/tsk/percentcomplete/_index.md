---
title: "Tsk.PercentComplete"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Lo stato attuale di un'attività espresso come percentuale della durata dell'attività che è stata completata"
type: docs
weight: 880
url: /it/net/aspose.tasks/tsk/percentcomplete/
---
## Tsk.PercentComplete field

Lo stato attuale di un'attività, espresso come percentuale della durata dell'attività completata.

```csharp
public static readonly Key<int, TaskKey> PercentComplete;
```

## Esempi

Mostra come modificare l'avanzamento di un'attività aggiornando la percentuale di completamento dell'attività.

```csharp
var project = new Project();
Console.WriteLine("Project Calculation mode is Automatic: {0}", project.CalculationMode.Equals(CalculationMode.Automatic));

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(2));
task.Set(Tsk.PercentComplete, 50);

// Accedi alle attività e visualizza la percentuale di completamento
foreach (var tsk in project.RootTask.Children)
{
    Console.WriteLine(tsk.Get(Tsk.PercentComplete));
    Console.WriteLine(tsk.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(tsk.Get(Tsk.PhysicalPercentComplete));
}
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


