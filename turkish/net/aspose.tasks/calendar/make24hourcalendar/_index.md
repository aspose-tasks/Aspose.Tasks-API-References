---
title: "Calendar.Make24HourCalendar"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar yöntemi. Verilen Calendar'ı 24 Saatlik Takvim yapar. 24 Saatlik Takvim, haftanın her gününün 24 saat çalıştığı bir takvimdir."
type: docs
weight: 10
url: /tr/net/aspose.tasks/calendar/make24hourcalendar/
---
## Calendar.Make24HourCalendar method

Verilen takvimi 24 Saatlik Takvim yapar. 24 Saatlik Takvim, haftanın her gününün 24 saat çalıştığı bir takvimdir.

```csharp
public static Calendar Make24HourCalendar(Calendar calendar)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| takvim | Takvim | 24 Saatlik Takvim oluşturmak için Takvim. |

### Dönüş Değeri

24 Saatlik Takvim.

## Örnekler

24 saatlik bir takvim nasıl oluşturulacağını gösterir.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// 24 saat yazdırılacak
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

Yeni bir takvimin 24 saatlik takvime nasıl dönüştürüleceğini gösterir.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("24 Hours");
calendar = Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// 24 saat yazdırılacak
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

### Ayrıca Bakınız

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


