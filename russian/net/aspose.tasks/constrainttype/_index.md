---
title: "Перечисление ConstraintType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.ConstraintType. Задаёт ограничение на дату начала или завершения задачи"
type: docs
weight: 330
url: /ru/net/aspose.tasks/constrainttype/
---
## ConstraintType enumeration

Указывает ограничение даты начала или завершения задачи.

```csharp
public enum ConstraintType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Undefined | `-1` | Значение не было определено в оригинальном файле проекта. |
| AsSoonAsPossible | `0` | Даты [`Start`](../tsk/start/) и [`Finish`](../tsk/finish/) задачи [`Task`](../task/) планируются как можно скорее с учётом дат родительского [`Start`](../tsk/start/) и [`Finish`](../tsk/finish/) и учитывая [`TaskLinks`](../project/tasklinks/). |
| AsLateAsPossible | `1` | [`Start`](../tsk/start/) и [`Finish`](../tsk/finish/) даты задачи [`Task`](../task/) запланированы ALAP относительно родительских дат [`Start`](../tsk/start/) и [`Finish`](../tsk/finish/) и с учётом [`TaskLinks`](../project/tasklinks/). |
| MustStartOn | `2` | Должно начаться |
| MustFinishOn | `3` | Должно завершиться |
| StartNoEarlierThan | `4` | Начало не ранее чем |
| StartNoLaterThan | `5` | Начало не позже чем |
| FinishNoEarlierThan | `6` | Завершение не ранее чем |
| FinishNoLaterThan | `7` | Завершение не позже чем |

## Примечания

При экспорте в XML неопределённые значения будут удалены из результирующего XML.

## Примеры

Показывает, как установить ограничение &lt;see cref=\"Aspose.Tasks.ConstraintType\" /&gt; ConstraintType.AsSoonAsPossible для задачи.

```csharp
var project = new Project(DataDir + "Constraints/ConstraintAsLateAsPossible.mpp");

// Установить ограничение As Soon As Possible для задачи с Id 11
var task = project.RootTask.Children.GetById(11);
task.Set(Tsk.ConstraintType, ConstraintType.AsSoonAsPossible);

SaveOptions options = new PdfSaveOptions();
options.StartDate = project.Get(Prj.StartDate);
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "AsSoonAsPossible_out.pdf", options);
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


