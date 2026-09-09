---
title: "Enum MonthPosition"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.MonthPosition enum. Bir ay içindeki öğenin konumunu belirtir."
type: docs
weight: 1070
url: /tr/net/aspose.tasks/monthposition/
---
## MonthPosition enumeration

Bir ay içinde ay öğesinin konumunu belirtir.

```csharp
public enum MonthPosition
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Undefined | `-1` | Tanımsız ay konumunu gösterir. |
| First | `0` | İlk konum ay konumunu gösterir. |
| Second | `1` | İkinci konum ay konumunu gösterir. |
| Third | `2` | Üçüncü konum ay konumunu gösterir. |
| Fourth | `3` | Dördüncü konum ay konumunu gösterir. |
| Last | `4` | Son konum ay konumunu gösterir. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


