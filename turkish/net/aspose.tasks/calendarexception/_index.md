---
title: "CalendarException Sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.CalendarException sınıfı. Takvimde istisnai zaman dilimlerini temsil eder."
type: docs
weight: 250
url: /tr/net/aspose.tasks/calendarexception/
---
## CalendarException class

Takvimdeki olağanüstü zaman dilimlerini temsil eder.

```csharp
public sealed class CalendarException
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [CalendarException](calendarexception/)() | `CalendarException` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [DaysOfWeek](../../aspose.tasks/calendarexception/daysofweek/) { get; } | Bu nesne için DayTypeCollection'ı alır. İstisnanın geçerli olduğu haftanın günleri. |
| [DayWorking](../../aspose.tasks/calendarexception/dayworking/) { get; set; } | Belirtilen tarih veya gün türünün çalışıp çalışmadığını gösteren bir değeri alır veya ayarlar. |
| [EnteredByOccurrences](../../aspose.tasks/calendarexception/enteredbyoccurrences/) { get; set; } | Tekrarlama aralığının bir olay sayısı girilerek tanımlanıp tanımlanmadığını gösteren değeri alır veya ayarlar. False, tekrarlama aralığının bir bitiş tarihi girilerek tanımlandığını belirtir. |
| [FromDate](../../aspose.tasks/calendarexception/fromdate/) { get; set; } | İstisna zamanının başlangıcını alır veya ayarlar. |
| [Month](../../aspose.tasks/calendarexception/month/) { get; set; } | İstisna tekrarlamasının planlandığı ayı alır veya ayarlar. |
| [MonthDay](../../aspose.tasks/calendarexception/monthday/) { get; set; } | İstisna tekrarlamasının planlandığı ayın gününü alır veya ayarlar. |
| [MonthItem](../../aspose.tasks/calendarexception/monthitem/) { get; set; } | İstisna tekrarlamasının planlandığı ay öğesini alır veya ayarlar. |
| [MonthPosition](../../aspose.tasks/calendarexception/monthposition/) { get; set; } | Bir ay içinde ay öğesinin konumunu alır veya ayarlar. |
| [Name](../../aspose.tasks/calendarexception/name/) { get; set; } | İstisnanın adını alır veya ayarlar. |
| [Occurrences](../../aspose.tasks/calendarexception/occurrences/) { get; set; } | Takvim istisnasının geçerli olduğu olay sayısını alır veya ayarlar. |
| [ParentCalendar](../../aspose.tasks/calendarexception/parentcalendar/) { get; } | Bu nesne için üst takvimi alır. |
| [Period](../../aspose.tasks/calendarexception/period/) { get; set; } | İstisna için tekrarlama dönemini alır veya ayarlar. |
| [ToDate](../../aspose.tasks/calendarexception/todate/) { get; set; } | İstisna zamanının sonunu alır veya ayarlar. |
| [Type](../../aspose.tasks/calendarexception/type/) { get; set; } | İstisna tipini alır veya ayarlar. |
| [WorkingTimes](../../aspose.tasks/calendarexception/workingtimes/) { get; set; } | WorkingTimeCollection nesnesini alır veya ayarlar. Haftaiçi çalışılan zamanı tanımlayan çalışma zamanları koleksiyonu. En az bir çalışma zamanı bulunmalı ve beşten fazla olamaz. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [CheckException](../../aspose.tasks/calendarexception/checkexception/)(DateTime) | Belirtilen DateTime yapısının örneği istisna günü ise true döndürür. |
| [Delete](../../aspose.tasks/calendarexception/delete/)() | Exception örneğini üst takvim CalendarExceptionCollection nesnesinden siler. |
| [GetExceptionDates](../../aspose.tasks/calendarexception/getexceptiondates/)() | Takvim istisnasının geçerli olduğu tarihleri döndürür. |
| [GetWorkingTime](../../aspose.tasks/calendarexception/getworkingtime/)() | Takvim istisnası için çalışma süresini döndürür. |

## Örnekler

Takvim istisnalarını ekleme/kaldırma yöntemini gösterir.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// takvim oluştur
var calendar = project.Calendars.Add("Calendar1");

// tatil için hafta içi istisnası oluştur
var exception = new CalendarException();
exception.Name = "New Calendar Exception";
exception.EnteredByOccurrences = false;
exception.FromDate = new DateTime(2009, 12, 24, 0, 0, 0);
exception.ToDate = new DateTime(2009, 12, 31, 23, 59, 0);
exception.Type = CalendarExceptionType.Daily;
exception.Month = Month.December;

exception.DayWorking = false;

// tarihin istisnai olup olmadığını kontrol et
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2009, 12, 26, 8, 0, 0)));

calendar.Exceptions.Add(exception);

// bir istisna kaldır
var cal = project.Calendars.ToList()[0];
if (cal.Exceptions.Count > 1)
{
    var excToRemove = cal.Exceptions[0];
    cal.Exceptions.Remove(excToRemove);
}

// bir istisna ekle
var exception2 = new CalendarException();
exception2.FromDate = new System.DateTime(2009, 1, 1);
exception2.ToDate = new System.DateTime(2009, 1, 3);
cal.Exceptions.Add(exception2);

// istisnaları yazdır
foreach (var exc in cal.Exceptions)
{
    Console.WriteLine("Name: " + exc.Name);
    Console.WriteLine("From: " + exc.FromDate.ToShortDateString());
    Console.WriteLine("To: " + exc.ToDate.ToShortDateString());
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


