---
title: "Calendar.PrimaveraProperties"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Calendar. Mendapatkan objek yang berisi properti khusus Primavera untuk kalender yang dibaca dari format Primavera"
type: docs
weight: 100
url: /id/net/aspose.tasks/calendar/primaveraproperties/
---
## Calendar.PrimaveraProperties property

Mendapatkan objek yang berisi properti khusus Primavera untuk kalender yang dibaca dari format Primavera.

```csharp
public PrimaveraCalendarProperties PrimaveraProperties { get; }
```

## Contoh

Menampilkan cara membaca proyek dari file Primavera dan memeriksa properti khusus Primavera pada kalender.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// Mengembalikan proyek dengan UID khusus
var project = new Project(DataDir + "ScheduleOptions.xer", options);

var calendar = project.Calendars.GetByUid(178);

Console.WriteLine("Hours per day in '{0}' : {1}", calendar.Name, calendar.PrimaveraProperties.HoursPerDay);
```

### Lihat Juga

* class [PrimaveraCalendarProperties](../../primaveracalendarproperties/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


