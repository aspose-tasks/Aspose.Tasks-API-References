---
title: "Calendar.Uid"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar özelliği. Takvimin benzersiz tanımlayıcısını alır veya ayarlar"
type: docs
weight: 110
url: /tr/net/aspose.tasks/calendar/uid/
---
## Calendar.Uid property

Takvimin benzersiz tanımlayıcısını alır veya ayarlar.

```csharp
public int Uid { get; set; }
```

## Örnekler

Takvim bilgilerini nasıl alacağınızı gösterir.

```csharp
var project = new Project(DataDir + "RetrieveCalendarInfo.mpp");

// Takvim Bilgilerini Al
foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("Calendar UID: " + calendar.Uid);
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Ayrıca Bakınız

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


