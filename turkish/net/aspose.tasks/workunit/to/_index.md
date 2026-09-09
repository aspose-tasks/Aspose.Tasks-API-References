---
title: "WorkUnit.To"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "WorkUnit özelliği. To tarihini alır veya ayarlar"
type: docs
weight: 30
url: /tr/net/aspose.tasks/workunit/to/
---
## WorkUnit.To property

To tarihini alır veya ayarlar.

```csharp
public DateTime To { get; set; }
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


