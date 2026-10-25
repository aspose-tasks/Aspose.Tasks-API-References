---
title: "CalendarException.ToDate"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CalendarException özelliği. Alır veya ayarlar istisna süresinin sonunu"
type: docs
weight: 140
url: /tr/net/aspose.tasks/calendarexception/todate/
---
## CalendarException.ToDate property

İstisna zamanının sonunu alır veya ayarlar.

```csharp
public DateTime ToDate { get; set; }
```

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

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


