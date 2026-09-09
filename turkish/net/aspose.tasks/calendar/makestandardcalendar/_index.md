---
title: "Calendar.MakeStandardCalendar"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar yöntemi. Varsayılan standart takvimi oluşturur"
type: docs
weight: 30
url: /tr/net/aspose.tasks/calendar/makestandardcalendar/
---
## Calendar.MakeStandardCalendar method

Varsayılan standart takvimi oluşturur.

```csharp
public static Calendar MakeStandardCalendar(Calendar calendar)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| takvim | Takvim | Standart takvim oluşturulacak Calendar. |

### Dönüş Değeri

Pazartesi-Cuma olmak üzere 5 çalışma günü ve çalışma saatleri 8-12 ve 13-17 olan takvim.

## Örnekler

Standart bir takvim oluşturmanın nasıl yapılacağını gösterir.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeStandardCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// çalışma saatlerini göster
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

İstisna günleri içeren bir takvim oluşturmanın nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "project_update_test.mpp");
var calendar = project.Calendars.GetByName("Standard");

// Takvim bilgilerini güncelleyin
Calendar.MakeStandardCalendar(calendar);
calendar.Name = "Test calendar";
var exception = new CalendarException();
exception.Name = "Exception 1";
exception.FromDate = DateTime.Now;
exception.ToDate = DateTime.Now.AddDays(2);
exception.DayWorking = true;

exception.WorkingTimes.Add(new WorkingTime(9, 13));
exception.WorkingTimes.Add(new WorkingTime(14, 19));
exception.WorkingTimes.Add(new WorkingTime(20, 21));
calendar.Exceptions.Add(exception);

var exception2 = new CalendarException();
exception.Name = "Exception 2";
exception2.FromDate = DateTime.Now.AddDays(7);
exception2.ToDate = exception2.FromDate;
exception2.DayWorking = false;
calendar.Exceptions.Add(exception2);

project.Set(Prj.Calendar, calendar);

project.Save(OutDir + "WriteUpdatedCalendarDataToMPP_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


