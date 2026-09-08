---
title: "Tsk.Work"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Общее время, запланированное для задачи для всех назначенных ресурсов"
type: docs
weight: 1150
url: /ru/net/aspose.tasks/tsk/work/
---
## Tsk.Work field

Общее запланированное время задачи для всех назначенных ресурсов.

```csharp
public static readonly Key<Duration, TaskKey> Work;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.Work.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Work, project.GetWork(1));

Console.WriteLine("Work: " + task.Get(Tsk.Work));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


