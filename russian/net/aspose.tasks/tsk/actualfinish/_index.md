---
title: "Tsk.ActualFinish"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Дата завершения задачи."
type: docs
weight: 40
url: /ru/net/aspose.tasks/tsk/actualfinish/
---
## Tsk.ActualFinish field

Дата, когда задача была завершена.

```csharp
public static readonly Key<DateTime, TaskKey> ActualFinish;
```

## Примеры

Показывает, что даты проекта сбрасываются в режиме оценки.

```csharp
var project = new Project();

// создать новые задачи
var task1 = project.RootTask.Children.Add("Task1");
task1.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task1.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

var task2 = project.RootTask.Children.Add("Task2");
task2.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task2.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

project.Save(OutDir + "EvaluationDateTimeLimitations_out.xml", SaveFileFormat.Xml);
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


