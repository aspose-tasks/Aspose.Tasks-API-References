---
title: "WorkWeekCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "WorkWeekCollection yöntemi. Bu koleksiyon için bir enumerator döndürür"
type: docs
weight: 50
url: /tr/net/aspose.tasks/workweekcollection/getenumerator/
---
## WorkWeekCollection.GetEnumerator method

Bu koleksiyon için bir enumerator döndürür.

```csharp
public IEnumerator<WorkWeek> GetEnumerator()
```

### Dönüş Değeri

bu koleksiyon için bir yineleyici.

## Örnekler

Bir takvim için özel bir çalışma haftası oluşturmanın nasıl yapılacağını gösterir.

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

Console.WriteLine("Work Weeks Count: " + calendar.WorkWeeks.Count);
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

* class [WorkWeek](../../workweek/)
* class [WorkWeekCollection](../)
* namespace [Aspose.Tasks](../../workweekcollection/)
* assembly [Aspose.Tasks](../../../)


