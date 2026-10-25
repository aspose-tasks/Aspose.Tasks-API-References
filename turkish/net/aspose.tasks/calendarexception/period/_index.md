---
title: "CalendarException.Period"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CalendarException özelliği. İstisna için tekrarlama periyodunu alır veya ayarlar."
type: docs
weight: 130
url: /tr/net/aspose.tasks/calendarexception/period/
---
## CalendarException.Period property

İstisna için tekrarlama dönemini alır veya ayarlar.

```csharp
public int Period { get; set; }
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

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


