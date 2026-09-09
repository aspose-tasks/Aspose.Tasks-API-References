---
title: "WeekDayCollection.CopyTo"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "WeekDayCollection yöntemi. Koleksiyon içeriğini belirtilen indekste bir diziye kopyalar"
type: docs
weight: 60
url: /tr/net/aspose.tasks/weekdaycollection/copyto/
---
## WeekDayCollection.CopyTo method

Koleksiyon içeriğini belirtilen indekste bir diziye kopyalar.

```csharp
public void CopyTo(WeekDay[] array, int arrayIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| array | WeekDay[] | Kopyalanacak [`WeekDay`](../../weekday/) hedef dizisi |
| arrayIndex | Int32 | Kopyalama işlemi için başlangıç indeksi. |

## Örnekler

Hafta günü koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project();
var calendar = project.Calendars.GetByName("Standard");

// hafta günlerini temizle
calendar.WeekDays.Clear();

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
var saturday = WeekDay.CreateDefaultWorkingDay(DayType.Saturday);
var sunday = WeekDay.CreateDefaultWorkingDay(DayType.Sunday);

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

var fridayWorkingTimes = new List<WorkingTime> { new WorkingTime(new DateTime(2020, 4, 13, 8, 0, 0), new DateTime(2020, 4, 13, 12, 0, 0)) };

var friday = new WeekDay(DayType.Friday, fridayWorkingTimes);
if (calendar.WeekDays.Contains(friday))
{
    calendar.WeekDays.Insert(4, friday);
}

Console.WriteLine("Calendar: " + calendar.Name);
Console.WriteLine("Week days count: " + calendar.WeekDays.Count);
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType);
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine("From: " + workingTime.From);
        Console.WriteLine("To: " + workingTime.To);
        Console.WriteLine();
    }
}

// cumartesi hafta gününü kaldır
calendar.WeekDays.RemoveAt(5);

// pazar hafta gününü kaldır
if (calendar.WeekDays.IndexOf(saturday) > 0)
{
    calendar.WeekDays.Remove(sunday);
}

Console.WriteLine("Working times after weekend was removed: ");
List<WeekDay> weekDays = calendar.WeekDays.ToList();
foreach (var day in weekDays)
{
    Console.WriteLine(day.DayType);
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine("From: " + workingTime.From);
        Console.WriteLine("To: " + workingTime.To);
        Console.WriteLine();
    }
}

var hour24Calendar = project.Calendars.Add("24 Hours");
Calendar.Make24HourCalendar(hour24Calendar);

// hafta günlerini kopyala
var weekDaysArray = new WeekDay[calendar.WeekDays.Count];
calendar.WeekDays.CopyTo(weekDaysArray, 0);

foreach (var weekDay in weekDaysArray)
{
    hour24Calendar.WeekDays.Add(weekDay);
}
```

### Ayrıca Bakınız

* class [WeekDay](../../weekday/)
* class [WeekDayCollection](../)
* namespace [Aspose.Tasks](../../weekdaycollection/)
* assembly [Aspose.Tasks](../../../)


