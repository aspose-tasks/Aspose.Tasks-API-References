---
title: "Tsk.OvertimeCost"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De totale overurenkost voor een taak voor een resource op alle toegewezen taken of voor een resource-toewijzing"
type: docs
weight: 860
url: /nl/net/aspose.tasks/tsk/overtimecost/
---
## Tsk.OvertimeCost field

De totale overurenkost voor een taak, voor een resource op alle toegewezen taken, of voor een resource-toewijzing.

```csharp
public static readonly Key<decimal, TaskKey> OvertimeCost;
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
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


