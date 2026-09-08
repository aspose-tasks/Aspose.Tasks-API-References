---
title: "Tsk.FreeSlackTimeSpan"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Время, на которое задача может быть отложена без задержки последующих задач"
type: docs
weight: 450
url: /ru/net/aspose.tasks/tsk/freeslacktimespan/
---
## Tsk.FreeSlackTimeSpan field

Время, на которое задачу можно отложить без задержки последующих задач.

```csharp
public static readonly Key<TimeSpan, TaskKey> FreeSlackTimeSpan;
```

## Примеры

Показывает, как читать свойство Tsk.FreeSlackTimeSpan. Свойство вычисляется, поэтому обычно нет необходимости задавать его явно.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Free Slack: " + task.Get(Tsk.FreeSlackTimeSpan));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


