---
title: "WorkingTimeCollection sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.WorkingTimeCollection sınıfı. WorkingTimeCollection nesnelerinin bir koleksiyonunu temsil eder"
type: docs
weight: 3670
url: /tr/net/aspose.tasks/workingtimecollection/
---
## WorkingTimeCollection class

`WorkingTimeCollection` nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class WorkingTimeCollection : IList<WorkingTime>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/workingtimecollection/count/) { get; } | Bu `WorkingTimeCollection` nesnesinde bulunan nesne sayısını alır. |
| [Item](../../aspose.tasks/workingtimecollection/item/) { get; set; } | Belirtilen indeksteki öğeyi döndürür. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/workingtimecollection/add/)(WorkingTime) | Bu koleksiyona yeni bir WorkingTime örneği ekler. |
| [Clear](../../aspose.tasks/workingtimecollection/clear/)() | Koleksiyondan tüm [`WorkingTime`](../workingtime/) öğelerini kaldırır. |
| [Contains](../../aspose.tasks/workingtimecollection/contains/)(WorkingTime) | Belirtilen öğenin Listede olup olmadığını kontrol eder. Doğrusal O(n) arama gerçekleştirir. |
| [CopyTo](../../aspose.tasks/workingtimecollection/copyto/)(WorkingTime[], int) | Bir koleksiyon içeriğini belirli bir indeksten başlayarak bir Array'e kopyalar |
| [GetEnumerator](../../aspose.tasks/workingtimecollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [Remove](../../aspose.tasks/workingtimecollection/remove/)(WorkingTime) | Bu koleksiyondan [`WorkingTime`](../workingtime/) örneğini kaldırır. |
| [ToList](../../aspose.tasks/workingtimecollection/tolist/)() | WorkingTimeCollection nesnesini [`WorkingTime`](../workingtime/) nesnelerinin bir listesine dönüştürür. |

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

* class [WorkingTime](../workingtime/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


