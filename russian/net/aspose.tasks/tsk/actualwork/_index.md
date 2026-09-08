---
title: "Tsk.ActualWork"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Tsk field. Объём работы, уже выполненной ресурсами, назначенными на задачи"
type: docs
weight: 90
url: /ru/net/aspose.tasks/tsk/actualwork/
---
## Tsk.ActualWork field

Объём работы, уже выполненной ресурсами, назначенными на задачи.

```csharp
public static readonly Key<Duration, TaskKey> ActualWork;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.ActualWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + task.Get(Tsk.ActualWork));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


