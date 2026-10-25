---
title: "WorkUnit.WorkingHours"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "WorkUnit özelliği. Çalışma saatlerinin süresini alır veya ayarlar"
type: docs
weight: 40
url: /tr/net/aspose.tasks/workunit/workinghours/
---
## WorkUnit.WorkingHours property

Çalışma saatlerinin süresini alır veya ayarlar.

```csharp
public TimeSpan WorkingHours { get; set; }
```

## Örnekler

Work unit bilgileriyle nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// Belirli bir tarih için çalışma saatlerini al.
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

Console.WriteLine("From: " + workUnit.From);
Console.WriteLine("To: " + workUnit.To);
Console.WriteLine("Working hours: " + workUnit.WorkingHours);
```

### Ayrıca Bakınız

* class [WorkUnit](../)
* namespace [Aspose.Tasks](../../workunit/)
* assembly [Aspose.Tasks](../../../)


