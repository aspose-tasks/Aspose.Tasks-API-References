---
title: "Tsk.ActualCost"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Kosten die zijn gemaakt voor reeds uitgevoerd werk door resources op hun taken, samen met eventuele andere geregistreerde kosten die aan de taak zijn gekoppeld"
type: docs
weight: 20
url: /nl/net/aspose.tasks/tsk/actualcost/
---
## Tsk.ActualCost field

Kosten die ontstaan voor werk dat al door resources op hun taken is uitgevoerd, samen met alle andere geregistreerde kosten die aan de taak zijn gekoppeld.

```csharp
public static readonly Key<decimal, TaskKey> ActualCost;
```

## Voorbeelden

Toont hoe de werkelijke eigenschappen van een taak gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "ActualTaskProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Alle verzamelde taken doorlopen
foreach (var task in collector.Tasks)
{
    Console.WriteLine("Task Name : " + task.Get(Tsk.Name));
    Console.WriteLine("Actual Start: " + task.Get(Tsk.ActualStart).ToLongDateString());
    Console.WriteLine("Actual Finish: " + task.Get(Tsk.ActualFinish).ToLongDateString());
    Console.WriteLine("Actual Duration: " + task.Get(Tsk.ActualDuration).TimeSpan.Hours);
    Console.WriteLine("Actual Cost: " + task.Get(Tsk.ActualCost));
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


