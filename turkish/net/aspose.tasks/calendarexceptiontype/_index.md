---
title: "Enum CalendarExceptionType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.CalendarExceptionType enum'ı. Takvim istisna türünü belirtir"
type: docs
weight: 270
url: /tr/net/aspose.tasks/calendarexceptiontype/
---
## CalendarExceptionType enumeration

Takvim istisna tipini belirtir.

```csharp
public enum CalendarExceptionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Daily | `0` | Günlük istisna türünü gösterir. |
| YearlyByDay | `1` | Ayın gününe göre yıllık istisna türünü gösterir. |
| YearlyByPosition | `2` | Pozisyona göre yıllık istisna türünü gösterir. |
| MonthlyByDay | `3` | Ayın gününe göre aylık istisna türünü gösterir. |
| MonthlyByPosition | `4` | Pozisyona göre aylık istisna türünü gösterir. |
| Weekly | `5` | Haftalık istisna türünü gösterir. |
| ByDayCount | `6` | Gün sayısına göre istisna türünü gösterir. |
| ByWeekDayCount | `7` | Haftanın gün sayısına göre istisna türünü gösterir. |
| NoExceptionType | `8` | İstisna türü olmadığını gösterir. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


