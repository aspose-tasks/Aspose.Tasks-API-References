---
title: "Tsk.ActualOvertimeWork"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Фактическое количество сверхурочной работы, уже выполненной ресурсами, назначенными на задачи"
type: docs
weight: 60
url: /ru/net/aspose.tasks/tsk/actualovertimework/
---
## Tsk.ActualOvertimeWork field

Фактическое количество сверхурочной работы, уже выполненной ресурсами, назначенными на задачи.

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWork;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.ActualOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + task.Get(Tsk.ActualOvertimeWork));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


