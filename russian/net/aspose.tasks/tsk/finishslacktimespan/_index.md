---
title: "Tsk.FinishSlackTimeSpan"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Продолжительность между датами раннего завершения и позднего завершения"
type: docs
weight: 400
url: /ru/net/aspose.tasks/tsk/finishslacktimespan/
---
## Tsk.FinishSlackTimeSpan field

Продолжительность между датами раннего завершения и позднего завершения.

```csharp
public static readonly Key<TimeSpan, TaskKey> FinishSlackTimeSpan;
```

## Примеры

Показывает, как читать свойство Tsk.FinishSlackTimeSpan. Свойство вычисляется, поэтому обычно нет необходимости задавать его явно.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Finish Slack: " + task.Get(Tsk.FinishSlackTimeSpan));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


