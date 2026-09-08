---
title: "Tsk.RemainingWork"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Время, всё ещё необходимое для завершения задачи или набора задач"
type: docs
weight: 990
url: /ru/net/aspose.tasks/tsk/remainingwork/
---
## Tsk.RemainingWork field

Время, необходимое для завершения задачи или набора задач.

```csharp
public static readonly Key<Duration, TaskKey> RemainingWork;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.RemainingWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + task.Get(Tsk.RemainingWork));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


