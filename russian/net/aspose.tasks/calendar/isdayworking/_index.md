---
title: "Calendar.IsDayWorking"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Calendar. Определяет, является ли указанный день рабочим согласно календарю"
type: docs
weight: 260
url: /ru/net/aspose.tasks/calendar/isdayworking/
---
## Calendar.IsDayWorking method

Определяет, является ли указанный день рабочим согласно календарю.

```csharp
public bool IsDayWorking(DateTime dt)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dt | DateTime | Дата, которую нужно проверить, является ли день рабочим. |

### Возвращаемое значение

True, если день является рабочим.

## Примеры

Показывает, как рассчитать рабочие часы.

```csharp
var project = new Project(DataDir + "CalculateWorkHours.mpp");

// Доступ к задаче по идентификатору
var task = project.RootTask.Children.GetById(1);

// Доступ к календарю и его начальной и конечной датам
var taskCalendar = task.Get(Tsk.Calendar);
var startDate = task.Get(Tsk.Start);
var endDate = task.Get(Tsk.Finish);

// Доступ к ресурсу и его календарю
var resource = project.Resources.GetByUid(1);
var resourceCalendar = resource.Get(Rsc.Calendar);

TimeSpan timeSpan;

// Получить продолжительность в минутах
double durationInMins = 0;
var tempDate = startDate;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        durationInMins += timeSpan.TotalMinutes;
    }

    tempDate = tempDate.AddDays(1);
}

tempDate = startDate;

// Получить продолжительность в часах
double durationInHours = 0;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        durationInHours += timeSpan.TotalHours;
    }

    tempDate = tempDate.AddDays(1);
}

// Получить продолжительность в днях
double durationInDays = 0;
tempDate = startDate;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        if (timeSpan.TotalHours > 0)
        {
            durationInDays += timeSpan.TotalDays * (24 / timeSpan.TotalHours);
        }
    }

    tempDate = tempDate.AddDays(1);
}

Console.WriteLine("Duration in Minutes = " + durationInMins);
Console.WriteLine("Duration in Hours = " + durationInHours);
Console.WriteLine("Duration in Days = " + durationInDays);
```

### См. также

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


