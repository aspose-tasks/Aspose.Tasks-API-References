---
title: "Calendar.PrimaveraProperties"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar özelliği. Primavera formatlarından okunan bir takvim için Primavera'ye özgü özellikleri içeren bir nesne alır"
type: docs
weight: 100
url: /tr/net/aspose.tasks/calendar/primaveraproperties/
---
## Calendar.PrimaveraProperties property

Primavera formatlarından okunan bir takvim için Primavera'ya özgü özellikleri içeren bir nesneyi alır.

```csharp
public PrimaveraCalendarProperties PrimaveraProperties { get; }
```

## Örnekler

Bir Primavera dosyasından bir projeyi nasıl okuyacağınızı ve takvimin Primavera'ye özgü özelliklerini nasıl inceleyeceğinizi gösterir.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// Özel UID'ye sahip projeyi döndürür
var project = new Project(DataDir + "ScheduleOptions.xer", options);

var calendar = project.Calendars.GetByUid(178);

Console.WriteLine("Hours per day in '{0}' : {1}", calendar.Name, calendar.PrimaveraProperties.HoursPerDay);
```

### Ayrıca Bakınız

* class [PrimaveraCalendarProperties](../../primaveracalendarproperties/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


