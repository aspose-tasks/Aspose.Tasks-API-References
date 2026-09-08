---
title: "Calendar.GetTaskFinishDateFromDuration"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Calendar. Вычисляет дату и время завершения задачи на основе её даты начала, разбитой на части, и продолжительности работы"
type: docs
weight: 210
url: /ru/net/aspose.tasks/calendar/gettaskfinishdatefromduration/
---
## Calendar.GetTaskFinishDateFromDuration method

Вычисляет дату и время завершения задачи на основе её даты начала, разбитых частей и длительности работы.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| задача | Задача | Задача, для которой вычисляется дата завершения. |
| продолжительность | TimeSpan | Продолжительность для вычисления. |

### Возвращаемое значение

Дата завершения задачи для заданных даты начала и продолжительности.

## Примечания

Возвращает DateTime.MinValue, если задача является сводной, null или её дата начала не установлена.

## Примеры

Показывает, как вычислить дату завершения задачи с помощью пользовательской длительности.

```csharp
var project = new Project(DataDir + "SplitTaskFinishDate.mpp");

// Найти разделённую задачу
var task = project.RootTask.Children.GetByUid(4);

// Найти календарь проекта
var calendar = project.Get(Prj.Calendar);

// Вычислить дату завершения задачи с различными длительностями
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 8 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(8, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 16 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(16, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 24 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(24, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 28 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(28, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 32 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(32, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 46 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(46, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 61 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(61, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 75 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(75, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 80 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(80, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 120 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(120, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 150 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(150, 0, 0)));
```

### См. также

* class [Task](../../task/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


