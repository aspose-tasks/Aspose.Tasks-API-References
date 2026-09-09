---
title: "CalendarException.EnteredByOccurrences"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CalendarException özelliği. Tekrarlama aralığının bir sayı girilerek tanımlanıp tanımlanmadığını gösteren bir değeri alır veya ayarlar. False, tekrarlama aralığının bir bitiş tarihi girilerek tanımlandığını belirtir."
type: docs
weight: 40
url: /tr/net/aspose.tasks/calendarexception/enteredbyoccurrences/
---
## CalendarException.EnteredByOccurrences property

Tekrarlama aralığının bir olay sayısı girilerek tanımlanıp tanımlanmadığını gösteren değeri alır veya ayarlar. False, tekrarlama aralığının bir bitiş tarihi girilerek tanımlandığını belirtir.

```csharp
public bool EnteredByOccurrences { get; set; }
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


