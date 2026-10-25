---
title: "WorkUnit.WorkUnit"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "WorkUnit yapıcı. WorkUnit sınıfının yeni bir örneğini başlatır. Belirtilen From ve To tarihleriyle yeni WorkUnit nesnesi oluşturur."
type: docs
weight: 10
url: /tr/net/aspose.tasks/workunit/workunit/
---
## WorkUnit constructor

[`WorkUnit`](../) sınıfının yeni bir örneğini başlatır. Belirtilen From ve To tarihleriyle yeni WorkUnit nesnesi oluşturur.

```csharp
public WorkUnit(DateTime from, DateTime to)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlangıç | DateTime | Çalışma saatlerinin başlangıç tarihi. |
| ile | DateTime | Çalışma saatlerinin bitiş tarihi. |

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


