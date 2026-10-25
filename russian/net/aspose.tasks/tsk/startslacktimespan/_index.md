---
title: "Tsk.StartSlackTimeSpan"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Продолжительность между датами раннего начала и позднего начала"
type: docs
weight: 1020
url: /ru/net/aspose.tasks/tsk/startslacktimespan/
---
## Tsk.StartSlackTimeSpan field

Продолжительность между датами раннего начала и позднего начала.

```csharp
public static readonly Key<TimeSpan, TaskKey> StartSlackTimeSpan;
```

## Примеры

Показывает, как читать свойство Tsk.StartSlackTimeSpan. Свойство вычисляется, поэтому обычно нет необходимости задавать его явно.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Start Slack: " + task.Get(Tsk.StartSlackTimeSpan));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


