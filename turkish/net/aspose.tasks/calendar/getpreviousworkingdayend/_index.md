---
title: "Calendar.GetPreviousWorkingDayEnd"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar yöntemi. Belirtilen tarihten önceki çalışma gününün sonunu hesaplar"
type: docs
weight: 190
url: /tr/net/aspose.tasks/calendar/getpreviousworkingdayend/
---
## Calendar.GetPreviousWorkingDayEnd method

Belirtilen tarihten önceki çalışma gününün sonunu hesaplar.

```csharp
public DateTime GetPreviousWorkingDayEnd(DateTime date)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tarih | DateTime | Önceki çalışma gününün sonunu hesaplamak için tarih. |

### Dönüş Değeri

Önceki çalışma gününün sonu.

## Örnekler

Bir takvim kullanarak önceki çalışma gününün sonunu nasıl alacağınızı gösterir.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// önceki çalışma gününün sonunu al
var previousWorkingDayEnd = calendar.GetPreviousWorkingDayEnd(new DateTime(2020, 4, 10, 13, 0, 0));

// 9 Nisan 2020 18:00 PM yazdırılacak
Console.WriteLine(previousWorkingDayEnd);
```

### Ayrıca Bakınız

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


