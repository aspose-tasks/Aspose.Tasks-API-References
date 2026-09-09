---
title: "Sınıf WorkUnit"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.WorkUnit sınıfı. Çalışma saatlerini temsil eder."
type: docs
weight: 3630
url: /tr/net/aspose.tasks/workunit/
---
## WorkUnit class

Çalışma saatlerini temsil eder.

```csharp
public class WorkUnit
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [WorkUnit](workunit/)(DateTime, DateTime) | `WorkUnit` sınıfının yeni bir örneğini başlatır. Belirtilen From ve To tarihleriyle yeni bir WorkUnit nesnesi oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [From](../../aspose.tasks/workunit/from/) { get; set; } | From tarihini alır veya ayarlar. |
| [To](../../aspose.tasks/workunit/to/) { get; set; } | To tarihini alır veya ayarlar. |
| [WorkingHours](../../aspose.tasks/workunit/workinghours/) { get; set; } | Çalışma saatlerinin süresini alır veya ayarlar. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


