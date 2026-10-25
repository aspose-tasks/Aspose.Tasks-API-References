---
title: "Sınıf WorkWeek"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.WorkWeek sınıfı. WorkWeek sınıfını temsil eder"
type: docs
weight: 3640
url: /tr/net/aspose.tasks/workweek/
---
## WorkWeek class

WorkWeek sınıfını temsil eder.

```csharp
public class WorkWeek
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [WorkWeek](workweek/)() | `WorkWeek` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [FromDate](../../aspose.tasks/workweek/fromdate/) { get; set; } | İş haftasının başlangıç DateTime'ını alır veya ayarlar |
| [Name](../../aspose.tasks/workweek/name/) { get; set; } | İş haftasının adını alır veya ayarlar |
| [ToDate](../../aspose.tasks/workweek/todate/) { get; set; } | İş haftasının bitiş DateTime'ını alır veya ayarlar |
| [WeekDays](../../aspose.tasks/workweek/weekdays/) { get; } | Hafta günlerini alır. |

## Örnekler

Projeden iş haftası bilgilerini nasıl okuyacağını gösterir.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Standard");
Calendar.MakeStandardCalendar(calendar);

var item = new WorkWeek();
item.Name = "My Work Week";
item.FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
item.ToDate = new DateTime(2020, 4, 17, 17, 0, 0);
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
item.WeekDays.Add(new WeekDay(DayType.Saturday));
item.WeekDays.Add(new WeekDay(DayType.Sunday));
calendar.WorkWeeks.Add(item);

Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);
foreach (var workWeek in calendar.WorkWeeks)
{
    // İş haftası adını, üst takvim adını, başlangıç ve bitiş tarihlerini görüntüle
    Console.WriteLine("Name: " + workWeek.Name);
    Console.WriteLine("Parent calendar name: " + calendar.Name);
    Console.WriteLine("From Date: " + workWeek.FromDate);
    Console.WriteLine("To Date: " + workWeek.ToDate);
    Console.WriteLine();

    // Bu veri, "Details." düğmesiyle ilgilidir; özel bir Hafta Günü için özel çalışma zamanları ayarlayabilir veya hatta çalışmaz olarak işaretleyebilirsiniz.
    List<WeekDay> weekDays = workWeek.WeekDays.ToList();
    foreach (var day in weekDays)
    {
        Console.WriteLine(day.DayType.ToString());

        // Çalışma zamanları arasında daha fazla dolaşabilir ve bunları görüntüleyebilirsiniz.
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }

    Console.WriteLine();
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


