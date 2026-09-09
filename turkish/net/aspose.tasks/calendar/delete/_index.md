---
title: "Calendar.Delete"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar yöntemi. Takvimi projeden kaldırır"
type: docs
weight: 140
url: /tr/net/aspose.tasks/calendar/delete/
---
## Calendar.Delete method

Takvimi projeden kaldırır.

```csharp
public void Delete()
```

## Örnekler

Bir projeden takvim silmenin nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "BrokenCalendar.mpp");

// takvimi isimle al
var calendar = project.Calendars.GetByName("Broken Calendar");

// takvimi sil
calendar.Delete();
```

### Ayrıca Bakınız

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


