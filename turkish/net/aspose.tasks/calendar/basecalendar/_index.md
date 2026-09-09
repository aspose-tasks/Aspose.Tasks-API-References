---
title: "Calendar.BaseCalendar"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar özelliği. Bu takvimin bağlı olduğu temel takvimi alır veya ayarlar. Yalnızca takvim bir temel takvim değilse uygulanır."
type: docs
weight: 40
url: /tr/net/aspose.tasks/calendar/basecalendar/
---
## Calendar.BaseCalendar property

Bu takvimin bağlı olduğu temel takvimi alır veya ayarlar. Yalnızca takvim bir temel takvim değilse uygulanabilir.

```csharp
public Calendar BaseCalendar { get; set; }
```

## Örnekler

Kaynağın takviminin temel takvimiyle nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var resource = project.Resources.Add("Resource1");

// Standart takvim ekle ve kaynağa ata
var calendar = project.Calendars.Add("Resource1");
resource.Set(Rsc.Calendar, calendar);

// Tüm kaynaklar için temel takvim adını göster
foreach (var rsc in project.Resources)
{
    if (rsc.Get(Rsc.Name) != null)
    {
        Console.WriteLine(rsc.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### Ayrıca Bakınız

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


