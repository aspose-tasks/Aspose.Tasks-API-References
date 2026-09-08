---
title: "Tsk.RegularWork"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Общее количество работы без сверхурочных, запланированной для выполнения ресурсами"
type: docs
weight: 940
url: /ru/net/aspose.tasks/tsk/regularwork/
---
## Tsk.RegularWork field

Общее количество работы без сверхурочных, запланированной для выполнения ресурсами.

```csharp
public static readonly Key<Duration, TaskKey> RegularWork;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.RegularWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + task.Get(Tsk.RegularWork));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


