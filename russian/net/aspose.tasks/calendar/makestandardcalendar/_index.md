---
title: "Calendar.MakeStandardCalendar"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Calendar. Создаёт стандартный календарь по умолчанию."
type: docs
weight: 30
url: /ru/net/aspose.tasks/calendar/makestandardcalendar/
---
## Calendar.MakeStandardCalendar method

Создает стандартный календарь по умолчанию.

```csharp
public static Calendar MakeStandardCalendar(Calendar calendar)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| календарь | Calendar | Календарь, из которого создаётся стандартный календарь. |

### Возвращаемое значение

Календарь с 5 рабочими днями (понедельник‑пятница) и рабочими часами 8‑12 и 13‑17.

## Примеры

Показывает, как создать стандартный календарь.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeStandardCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// показать рабочие часы
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

Показывает, как создать календарь с исключительными днями.

```csharp
var project = new Project(DataDir + "project_update_test.mpp");
var calendar = project.Calendars.GetByName("Standard");

// Обновить информацию о календаре
Calendar.MakeStandardCalendar(calendar);
calendar.Name = "Test calendar";
var exception = new CalendarException();
exception.Name = "Exception 1";
exception.FromDate = DateTime.Now;
exception.ToDate = DateTime.Now.AddDays(2);
exception.DayWorking = true;

exception.WorkingTimes.Add(new WorkingTime(9, 13));
exception.WorkingTimes.Add(new WorkingTime(14, 19));
exception.WorkingTimes.Add(new WorkingTime(20, 21));
calendar.Exceptions.Add(exception);

var exception2 = new CalendarException();
exception.Name = "Exception 2";
exception2.FromDate = DateTime.Now.AddDays(7);
exception2.ToDate = exception2.FromDate;
exception2.DayWorking = false;
calendar.Exceptions.Add(exception2);

project.Set(Prj.Calendar, calendar);

project.Save(OutDir + "WriteUpdatedCalendarDataToMPP_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


