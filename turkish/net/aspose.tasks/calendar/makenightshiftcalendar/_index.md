---
title: "Calendar.MakeNightShiftCalendar"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar yöntemi. Verilen takvimi Gece Vardiyası Takvimi olarak oluşturur"
type: docs
weight: 20
url: /tr/net/aspose.tasks/calendar/makenightshiftcalendar/
---
## Calendar.MakeNightShiftCalendar method

Verilen Takvimi Gece Vardiyası Takvimi yapar.

```csharp
public static Calendar MakeNightShiftCalendar(Calendar calendar)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| takvim | Takvim | Gece Vardiyası Takvimi oluşturmak için Takvim. |

### Dönüş Değeri

Gece Vardiyası Takvimi.

## Örnekler

Gece vardiyası takvimi oluşturmanın nasıl yapılacağını gösterir.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// çalışma saatlerini göster
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

Bir takvimi gece vardiyası takvimine dönüştürmenin nasıl yapılacağını gösterir.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("Night Shift");
calendar = Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// çalışma saatlerini göster
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

### Ayrıca Bakınız

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


