---
title: "Tsk.BCWS"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. De cumulatieve tijdsgephaseerde baselinekosten tot de statusdatum of de datum van vandaag"
type: docs
weight: 130
url: /nl/net/aspose.tasks/tsk/bcws/
---
## Tsk.BCWS field

De cumulatieve tijdsfase-basiskosten tot de statusdatum of de datum van vandaag.

```csharp
public static readonly Key<double, TaskKey> BCWS;
```

## Voorbeelden

Toont hoe taakkostwaarden gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

foreach (var task in collector.Tasks)
{
    Console.WriteLine("Cost: " + task.Get(Tsk.Cost));
    Console.WriteLine("ACWP: " + task.Get(Tsk.ACWP));
    Console.WriteLine("BCWP: " + task.Get(Tsk.BCWP));
    Console.WriteLine("BCWS: " + task.Get(Tsk.BCWS));

    // CV = BCWP - ACWP
    Console.WriteLine("CV: " + task.Get(Tsk.CV));
    Console.WriteLine();
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


