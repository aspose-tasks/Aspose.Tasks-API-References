---
title: "Sınıf WeekDay"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.WeekDay sınıfı. Bir haftanın düzenli günlerini veya takvimdeki istisna günlerini tanımlayan bir hafta gününü temsil eder."
type: docs
weight: 3540
url: /tr/net/aspose.tasks/weekday/
---
## WeekDay class

Bir takvimde haftanın normal günlerini veya istisna günlerini tanımlayan bir hafta gününü temsil eder.

```csharp
public class WeekDay
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [WeekDay](weekday/#constructor)() | `WeekDay` sınıfının yeni bir örneğini başlatır. |
| [WeekDay](weekday/#constructor_1)(DayType) | `WeekDay` sınıfının yeni bir örneğini belirtilen gün türüyle başlatır. |
| [WeekDay](weekday/#constructor_3)(DayType, IEnumerable&lt;WorkingTime&gt;) | `WeekDay` sınıfının yeni bir örneğini belirtilen gün türü ve çalışma zaman dilimleri listesiyle başlatır. |
| [WeekDay](weekday/#constructor_2)(DayType, params WorkingTime[]) | `WeekDay` sınıfının yeni bir örneğini belirtilen gün türü ve çalışma zaman dilimleriyle başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [DayType](../../aspose.tasks/weekday/daytype/) { get; } | Bir günün türünü alır. |
| [DayWorking](../../aspose.tasks/weekday/dayworking/) { get; set; } | Belirtilen tarih veya gün türünün çalışıp çalışmadığını gösteren bir değeri alır veya ayarlar. |
| [FromDate](../../aspose.tasks/weekday/fromdate/) { get; set; } | Bir istisna zamanının başlangıcını alır veya ayarlar. |
| [ToDate](../../aspose.tasks/weekday/todate/) { get; set; } | Bir istisna zamanının sonunu alır veya ayarlar. |
| [WorkingTimes](../../aspose.tasks/weekday/workingtimes/) { get; } | Bu WeekDay örneği için WorkingTimeCollection'ı alır. Hafta içi çalışılan zamanı tanımlayan çalışma zamanları koleksiyonu. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [CreateDefaultWorkingDay](../../aspose.tasks/weekday/createdefaultworkingday/)(DayType) | Varsayılan çalışma gününü oluşturur. |
| [Clone](../../aspose.tasks/weekday/clone/)() | Hafta gününün derin bir kopyasını döndürür. |
| override [Equals](../../aspose.tasks/weekday/equals/)(object) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| override [GetHashCode](../../aspose.tasks/weekday/gethashcode/)() | `WeekDay` sınıfının örneği için bir hash kod değeri döndürür. |
| [GetWorkingTime](../../aspose.tasks/weekday/getworkingtime/)() | Bir hafta günü için çalışma zamanını döndürür. |
| static [CastToDayType](../../aspose.tasks/weekday/casttodaytype/)(DayOfWeek) | .Net'in DayOfWeek değerini [`DayType`](./daytype/) tipine dönüştürür. |
| static [SetDefaultWorkingTime](../../aspose.tasks/weekday/setdefaultworkingtime/)(WeekDay) | Belirtilen hafta günü için varsayılan zaman dilimlerini ayarlar. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


