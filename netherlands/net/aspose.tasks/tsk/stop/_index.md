---
title: "Tsk.Stop"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. De datum die het einde van het feitelijke gedeelte van een taak aangeeft"
type: docs
weight: 1060
url: /nl/net/aspose.tasks/tsk/stop/
---
## Tsk.Stop field

De datum die het einde van het daadwerkelijke gedeelte van een taak aangeeft.

```csharp
public static readonly Key<DateTime, TaskKey> Stop;
```

## Voorbeelden

Toont hoe de Stop/Resume-datums van een taak gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "StopResumeDates.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Controleer Stop- en Resume-datums voor alle taken
foreach (var task in collector.Tasks)
{
    if (task.Get(Tsk.Stop).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Stop: NA");
    }
    else
    {
        Console.WriteLine("Stop: " + task.Get(Tsk.Stop).ToShortDateString());
    }

    if (task.Get(Tsk.Resume).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Resume: NA");
    }
    else
    {
        Console.WriteLine("Resume: " + task.Get(Tsk.Resume).ToShortDateString());
    }
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


