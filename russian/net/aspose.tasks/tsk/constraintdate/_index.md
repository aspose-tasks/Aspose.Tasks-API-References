---
title: "Tsk.ConstraintDate"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Конкретная дата, связанная с типом ограничения"
type: docs
weight: 200
url: /ru/net/aspose.tasks/tsk/constraintdate/
---
## Tsk.ConstraintDate field

Конкретная дата, связанная с типом ограничения.

```csharp
public static readonly Key<DateTime, TaskKey> ConstraintDate;
```

## Примеры

Показывает, как получить/установить ограничение для задачи.

```csharp
var project = new Project(DataDir + "ConstraintAsLateAsPossible.mpp");

// Установить ограничение Как можно позже для задачи с Id 11
var newTask = project.RootTask.Children.GetById(11);
newTask.Set(Tsk.ConstraintType, ConstraintType.AsLateAsPossible);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Проанализировать все собранные задачи
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.ConstraintType).ToString());
    Console.WriteLine(task.Get(Tsk.ConstraintDate).ToShortDateString() == "1/1/2000" ? "NA" : task.Get(Tsk.ConstraintDate).ToShortDateString());
}

SaveOptions options = new PdfSaveOptions
{
    StartDate = project.Get(Prj.StartDate),
    Timescale = Timescale.ThirdsOfMonths
};

project.Save(OutDir + "SetConstraintAsLateAsPossible_out.pdf", options);
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


