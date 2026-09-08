---
title: "Tsk.OvertimeWork"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Количество сверхурочной работы, запланированной для выполнения всеми ресурсами, назначенными на задачу"
type: docs
weight: 870
url: /ru/net/aspose.tasks/tsk/overtimework/
---
## Tsk.OvertimeWork field

Количество сверхурочной работы, запланированной для выполнения всеми ресурсами, назначенными на задачу.

```csharp
public static readonly Key<Duration, TaskKey> OvertimeWork;
```

## Примеры

Показывает, как читать сверхурочные задачи.

```csharp
var project = new Project(DataDir + "TaskOvertimes.mpp");

// Читать сверхурочные и процент завершения задач
foreach (var task in project.RootTask.Children)
{
    Console.WriteLine(task.Get(Tsk.OvertimeCost));
    Console.WriteLine(task.Get(Tsk.OvertimeWork));
    Console.WriteLine(task.Get(Tsk.PercentComplete));
    Console.WriteLine(task.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(task.Get(Tsk.PhysicalPercentComplete));

    // Установить процент завершения
    task.Set(Tsk.PercentComplete, 100);
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


