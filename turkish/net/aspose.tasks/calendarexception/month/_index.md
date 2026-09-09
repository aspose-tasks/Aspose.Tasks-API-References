---
title: "CalendarException.Month"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CalendarException özelliği. Alır veya ayarlar bir istisna tekrarı planlanan ayı"
type: docs
weight: 60
url: /tr/net/aspose.tasks/calendarexception/month/
---
## CalendarException.Month property

İstisna tekrarlamasının planlandığı ayı alır veya ayarlar.

```csharp
public Month Month { get; set; }
```

## Örnekler

Ay günüyle takvim istisnasının nasıl tanımlanacağını gösterir.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// takvim oluştur
var calendar = project.Calendars.Add("Calendar1");

// her cuma için takvim istisnası oluştur
var exception = new CalendarException();
exception.Type = CalendarExceptionType.MonthlyByDay;
exception.FromDate = new DateTime(2010, 1, 1);
exception.ToDate = new DateTime(2020, 12, 31);
exception.Month = Month.December;
exception.MonthDay = 1;
exception.MonthItem = MonthItemType.Undefined;
exception.MonthPosition = MonthPosition.Last;
exception.Period = 5;

// bir cuma gününün istisnai olduğunu kontrol et
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2012, 12, 1)));

// istisnayı takvime ekle
calendar.Exceptions.Add(exception);
```

### Ayrıca Bakınız

* enum [Month](../../month/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


