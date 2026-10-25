---
title: "WorkingTimeCollection.Count"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "WorkingTimeCollection özelliği. Bu WorkingTimeCollection nesnesinde bulunan nesne sayısını alır"
type: docs
weight: 10
url: /tr/net/aspose.tasks/workingtimecollection/count/
---
## WorkingTimeCollection.Count property

Bu [`WorkingTimeCollection`](../) nesnesinde bulunan nesne sayısını alır.

```csharp
public int Count { get; }
```

## Örnekler

Working time koleksiyonuyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Custom Calendar");

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));

var saturdayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(8, 12),
    new WorkingTime(13, 15)
};
var saturday = new WeekDay(DayType.Saturday);
foreach (var time in saturdayWorkingTimes)
{
    saturday.WorkingTimes.Add(time);
}

// Cumartesi çalışma zamanlarını yazdır
Console.WriteLine("Saturday working period number: " + saturday.WorkingTimes.Count);
foreach (var time in saturday.WorkingTimes)
{
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

var sundayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(10, 15)
};
var sunday = new WeekDay(DayType.Sunday, sundayWorkingTimes);

// Pazar çalışma zamanlarını yazdır
List<WorkingTime> workingTimes = sunday.WorkingTimes.ToList();
Console.WriteLine("Sunday working period number: " + workingTimes.Count);
for (var index = 0; index < workingTimes.Count; index++)
{
    var time = workingTimes[index];
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType + ": ");

    // Çalışma zamanları arasında daha fazla dolaşabilir ve bunları görüntüleyebilirsiniz.
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine(workingTime.From);
        Console.WriteLine(workingTime.To);
    }

    Console.WriteLine();
}
```

### Ayrıca Bakınız

* class [WorkingTimeCollection](../)
* namespace [Aspose.Tasks](../../workingtimecollection/)
* assembly [Aspose.Tasks](../../../)


