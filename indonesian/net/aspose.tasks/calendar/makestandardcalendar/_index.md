---
title: "Calendar.MakeStandardCalendar"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Calendar. Membuat kalender standar default"
type: docs
weight: 30
url: /id/net/aspose.tasks/calendar/makestandardcalendar/
---
## Calendar.MakeStandardCalendar method

Membuat kalender standar default.

```csharp
public static Calendar MakeStandardCalendar(Calendar calendar)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| kalender | Calendar | Kalender untuk membuat kalender standar dari. |

### Nilai Kembali

Kalender dengan 5 hari kerja (Senin-Jumat) dengan jam kerja 8-12 dan 13-17.

## Contoh

Menampilkan cara membuat kalender standar.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeStandardCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// tampilkan jam kerja
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

Menampilkan cara membuat kalender dengan hari pengecualian.

```csharp
var project = new Project(DataDir + "project_update_test.mpp");
var calendar = project.Calendars.GetByName("Standard");

// Perbarui informasi kalender
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

### Lihat Juga

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


