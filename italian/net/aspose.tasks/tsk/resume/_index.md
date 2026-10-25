---
title: "Tsk.Resume"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La data in cui la parte rimanente di un'attività è programmata per riprendere dopo aver registrato qualsiasi progresso"
type: docs
weight: 1000
url: /it/net/aspose.tasks/tsk/resume/
---
## Tsk.Resume field

La data in cui la parte rimanente di un'attività è programmata per riprendere dopo aver registrato un progresso.

```csharp
public static readonly Key<DateTime, TaskKey> Resume;
```

## Esempi

Mostra come leggere le date di Stop/Resume dell'attività.

```csharp
var project = new Project(DataDir + "StopResumeDates.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Verifica le date di Stop e Resume per tutte le attività
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

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


