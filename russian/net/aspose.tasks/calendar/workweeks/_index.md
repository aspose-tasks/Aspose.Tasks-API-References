---
title: "Calendar.WorkWeeks"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Calendar. Возвращает объект WorkWeekCollections. Коллекцию рабочих недель, связанных с календарем"
type: docs
weight: 130
url: /ru/net/aspose.tasks/calendar/workweeks/
---
## Calendar.WorkWeeks property

Получает объект WorkWeekCollections. Коллекция рабочих недель, связанных с календарем.

```csharp
public WorkWeekCollection WorkWeeks { get; }
```

## Примеры

Показывает, как прочитать информацию о рабочей неделе.

```csharp
var project = new Project(DataDir + "WorkWithWorkWeekCollection.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var workWeek in calendar.WorkWeeks)
{
    // Отобразить название рабочей недели, даты начала и окончания
    var name = workWeek.Name;
    var fromDate = workWeek.FromDate;
    var toDate = workWeek.ToDate;
    Console.WriteLine("Name: " + name);
    Console.WriteLine("From Date: " + fromDate);
    Console.WriteLine("To Date: " + toDate);

    // Эти данные относятся к кнопке "Details." — здесь можно задать специальные рабочие часы для определённого дня недели или даже сделать его нерабочим.
    foreach (var day in workWeek.WeekDays)
    {
        // Вы можете дальше проходить по рабочим часам и отображать их.
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }
}
```

### См. также

* class [WorkWeekCollection](../../workweekcollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


