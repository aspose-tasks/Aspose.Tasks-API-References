---
title: "CalendarException.DaysOfWeek"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CalendarException özelliği. Bu nesne için DayTypeCollection'ı alır. İstisnanın geçerli olduğu haftanın günleri"
type: docs
weight: 20
url: /tr/net/aspose.tasks/calendarexception/daysofweek/
---
## CalendarException.DaysOfWeek property

Bu nesne için DayTypeCollection'ı alır. İstisnanın geçerli olduğu haftanın günleri.

```csharp
public DayTypeCollection DaysOfWeek { get; }
```

## Örnekler

Hafta gününe göre takvim istisnasının nasıl tanımlanacağını gösterir.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// takvim oluştur
var calendar = project.Calendars.Add("Calendar1");

// her cuma için takvim istisnası oluştur
var exception = new CalendarException();
exception.Type = CalendarExceptionType.Weekly;
exception.FromDate = new DateTime(2020, 4, 6);
exception.ToDate = new DateTime(2020, 4, 12);
exception.DaysOfWeek.Add(DayType.Friday);

// Cuma gününün istisnai olduğunu kontrol edin
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2020, 4, 10)));

// istisnayı takvime ekle
calendar.Exceptions.Add(exception);
```

### Ayrıca Bakınız

* class [DayTypeCollection](../../daytypecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


