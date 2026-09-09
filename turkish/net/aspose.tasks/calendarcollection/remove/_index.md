---
title: "CalendarCollection.Remove"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CalendarCollection yöntemi. Takvimi Project CalendarCollection'dan kaldırır"
type: docs
weight: 60
url: /tr/net/aspose.tasks/calendarcollection/remove/
---
## CalendarCollection.Remove method

Takvimi Proje CalendarCollection'dan kaldırır.

```csharp
public bool Remove(Calendar item)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| öğe | Takvim | Kaldırılacak takvim. |

### Dönüş Değeri

Kaldırılırsa true, aksi takdirde false döndürür.

### İstisnalar

| istisna | koşul |
| --- | --- |
| InvalidOperationException | Takvim kaldırılamadığında fırlatılır. |

## Örnekler

Koleksiyondaki bir takvimin nasıl değiştirileceğini gösterir.

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendar = project.Calendars.GetByName("TestCalendar");
if (calendar != null)
{
    project.Calendars.Remove(calendar);
}

// yeni takvim ekle
project.Calendars.Add("New Calendar");
project.Save(OutDir + "ReplaceCalendarWithNewCalendar_out.mpp", SaveFileFormat.Mpp);
```

### Ayrıca Bakınız

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


