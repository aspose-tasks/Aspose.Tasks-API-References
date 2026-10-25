---
title: "Calendar.GetNextWorkingDayStart"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar yöntemi. Belirtilen tarih için bir sonraki çalışma gününün başlangıcını hesaplar"
type: docs
weight: 180
url: /tr/net/aspose.tasks/calendar/getnextworkingdaystart/
---
## Calendar.GetNextWorkingDayStart method

Belirtilen tarih için bir sonraki çalışma gününün başlangıcını hesaplar.

```csharp
public DateTime GetNextWorkingDayStart(DateTime date)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tarih | DateTime | Bir sonraki çalışma gününün başlangıcını almak için tarih. |

### Dönüş Değeri

Bir sonraki çalışma gününün başlangıç DateTime'ı.

## Örnekler

Bir takvim kullanarak bir sonraki çalışma gününün başlangıcının nasıl alınacağını gösterir.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// bir sonraki çalışma gününün başlangıcını al (hafta sonu atlanır)
var nextWorkingDayStart = calendar.GetNextWorkingDayStart(new DateTime(2020, 4, 10, 13, 0, 0));

// 13 Nisan 2020 9:00 AM yazdırılacak
Console.WriteLine(nextWorkingDayStart);
```

### Ayrıca Bakınız

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


