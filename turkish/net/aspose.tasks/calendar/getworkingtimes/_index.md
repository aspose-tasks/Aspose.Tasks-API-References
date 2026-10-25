---
title: "Calendar.GetWorkingTimes"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar yöntemi. Belirtilen tarih için çalışma zamanlarının WorkingTimeCollection'ını döndürür"
type: docs
weight: 240
url: /tr/net/aspose.tasks/calendar/getworkingtimes/
---
## Calendar.GetWorkingTimes method

Belirtilen tarih için çalışma zamanlarının [`WorkingTimeCollection`](../../workingtimecollection/) koleksiyonunu döndürür.

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dt | DateTime | Çalışma saatlerini almak için tarih. |

### Dönüş Değeri

[`WorkingTime`](../../workingtime/) örneklerinin koleksiyonu.

## Örnekler

Belirli bir tarih için çalışma zamanlarını nasıl alacağınızı gösterir.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// belirli tarih için çalışma zamanlarını al
var workingTimes = calendar.GetWorkingTimes(new DateTime(2020, 4, 8, 8, 0, 0));

// 16 saat yazdırılacak
foreach (var workingTime in workingTimes)
{
    Console.WriteLine("From: " + workingTime.From);
    Console.WriteLine("To: " + workingTime.To);
}
```

### Ayrıca Bakınız

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


