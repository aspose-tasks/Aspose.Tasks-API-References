---
title: "Tsk.Stop"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Дата, представляющая конец фактической части задачи"
type: docs
weight: 1060
url: /ru/net/aspose.tasks/tsk/stop/
---
## Tsk.Stop field

Дата, представляющая окончание фактической части задачи.

```csharp
public static readonly Key<DateTime, TaskKey> Stop;
```

## Примеры

Показывает, как читать даты Stop/Resume задачи

```csharp
var project = new Project(DataDir + "StopResumeDates.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Проверьте даты Stop и Resume для всех задач
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

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


