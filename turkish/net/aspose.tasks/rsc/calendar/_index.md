---
title: "Rsc.Calendar"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynağın takvimi"
type: docs
weight: 190
url: /tr/net/aspose.tasks/rsc/calendar/
---
## Rsc.Calendar field

Bir kaynağın takvimi.

```csharp
public static readonly Key<Calendar, RscKey> Calendar;
```

## Örnekler

Bir kaynak takviminin nasıl alınacağını/ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var res = project.Resources.Add("Resource1");

// Standart takvim ekle ve kaynağa ata
var cal = project.Calendars.Add("Resource1");
res.Set(Rsc.Calendar, cal);

// Tüm kaynaklar için temel takvim adını göster
foreach (var resource in project.Resources)
{
    if (resource.Get(Rsc.Name) != null)
    {
        Console.WriteLine(resource.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


