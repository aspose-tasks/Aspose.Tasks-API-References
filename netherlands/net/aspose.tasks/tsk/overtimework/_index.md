---
title: "Tsk.OvertimeWork"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De hoeveelheid overwerk die gepland is om uitgevoerd te worden door alle aan een taak toegewezen resources"
type: docs
weight: 870
url: /nl/net/aspose.tasks/tsk/overtimework/
---
## Tsk.OvertimeWork field

De hoeveelheid overuren die gepland is om uitgevoerd te worden door alle resources die aan een taak zijn toegewezen.

```csharp
public static readonly Key<Duration, TaskKey> OvertimeWork;
```

## Voorbeelden

Toont hoe overuren van taken te lezen.

```csharp
var project = new Project(DataDir + "TaskOvertimes.mpp");

// Lees overuren en voltooiingspercentage voor taken
foreach (var task in project.RootTask.Children)
{
    Console.WriteLine(task.Get(Tsk.OvertimeCost));
    Console.WriteLine(task.Get(Tsk.OvertimeWork));
    Console.WriteLine(task.Get(Tsk.PercentComplete));
    Console.WriteLine(task.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(task.Get(Tsk.PhysicalPercentComplete));

    // Stel voltooiingspercentage in
    task.Set(Tsk.PercentComplete, 100);
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


