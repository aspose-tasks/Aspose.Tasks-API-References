---
title: "Calendar.Name"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar özelliği. Takvimin adını alır veya ayarlar"
type: docs
weight: 90
url: /tr/net/aspose.tasks/calendar/name/
---
## Calendar.Name property

Takvimin adını alır veya ayarlar.

```csharp
public string Name { get; set; }
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


