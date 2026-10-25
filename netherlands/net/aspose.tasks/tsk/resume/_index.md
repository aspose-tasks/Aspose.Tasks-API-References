---
title: "Tsk.Resume"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk field. De datum waarop het resterende deel van een taak is gepland om te hervatten nadat enige voortgang is ingevoerd"
type: docs
weight: 1000
url: /nl/net/aspose.tasks/tsk/resume/
---
## Tsk.Resume field

De datum waarop het resterende deel van een taak gepland is om te hervatten na het maken van enige voortgang.

```csharp
public static readonly Key<DateTime, TaskKey> Resume;
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


