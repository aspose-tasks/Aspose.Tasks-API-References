---
title: "WeekDay.FromDate"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "WeekDay özelliği. Bir istisna zamanının başlangıcını alır veya ayarlar"
type: docs
weight: 50
url: /tr/net/aspose.tasks/weekday/fromdate/
---
## WeekDay.FromDate property

Bir istisna zamanının başlangıcını alır veya ayarlar.

```csharp
public DateTime FromDate { get; set; }
```

## Örnekler

Hafta günlerini tanımlayarak yeni bir takvim oluşturmanın nasıl yapılacağını gösterir.

```csharp
var project = new Project();

// Bir takvim tanımla
var calendar = project.Calendars.Add("Calendar1");

// Pazartesiden perşembeye varsayılan zamanlarla çalışma günleri ekle
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// İstisna gününün başlangıç ve bitiş tarihlerini kontrol edin
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Cuma gününü kısa çalışma günü olarak ayarla

// Çalışma zamanını ayarlar. 
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// Bir <see cref="DayOfWeek" /> değerini <see cref="Aspose.Tasks.DayType" /> değerine dönüştürmenin bir yolu vardır.
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

// tüm çalışma zamanlarını yazdıralım
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### Ayrıca Bakınız

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


