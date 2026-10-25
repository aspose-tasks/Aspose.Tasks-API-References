---
title: "CalendarException.Occurrences"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CalendarException özelliği. Alır veya ayarlar takvim istisnasının geçerli olduğu tekrar sayısını"
type: docs
weight: 110
url: /tr/net/aspose.tasks/calendarexception/occurrences/
---
## CalendarException.Occurrences property

Takvim istisnasının geçerli olduğu olay sayısını alır veya ayarlar.

```csharp
public int Occurrences { get; set; }
```

## Örnekler

Takvim istisnasını oluşumlara göre nasıl tanımlayacağınızı gösterir.

```csharp
var project = new Project();

// Bir takvim tanımla
var calendar = project.Calendars.Add("Calendar1");

// İstisna tanımlayın ve oluşumları belirtin
var exception = new CalendarException();
exception.EnteredByOccurrences = true;
exception.Occurrences = 5;
exception.Type = CalendarExceptionType.YearlyByDay;
exception.MonthDay = 22;
exception.Month = Month.April;

// Takvime istisna ekle
calendar.Exceptions.Add(exception);
```

### Ayrıca Bakınız

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


