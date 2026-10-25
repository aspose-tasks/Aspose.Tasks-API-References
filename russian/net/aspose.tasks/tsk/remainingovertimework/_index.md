---
title: "Tsk.RemainingOvertimeWork"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Количество оставшегося запланированного сверхурочного времени"
type: docs
weight: 980
url: /ru/net/aspose.tasks/tsk/remainingovertimework/
---
## Tsk.RemainingOvertimeWork field

Количество оставшегося запланированного сверхурочного времени.

```csharp
public static readonly Key<Duration, TaskKey> RemainingOvertimeWork;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.RemainingOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + task.Get(Tsk.RemainingOvertimeWork));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


