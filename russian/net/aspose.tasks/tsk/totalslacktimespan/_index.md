---
title: "Tsk.TotalSlackTimeSpan"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Время, на которое дата завершения задачи может быть отложена без задержки даты завершения проекта"
type: docs
weight: 1090
url: /ru/net/aspose.tasks/tsk/totalslacktimespan/
---
## Tsk.TotalSlackTimeSpan field

Время, на которое можно отложить дату завершения задачи, не откладывая дату завершения проекта.

```csharp
public static readonly Key<TimeSpan, TaskKey> TotalSlackTimeSpan;
```

## Примеры

Показывает, как читать свойство Tsk.TotalSlackTimeSpan. Свойство вычисляется, поэтому обычно нет необходимости задавать его явно.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Total Slack: " + task.Get(Tsk.TotalSlackTimeSpan));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


