---
title: "CalendarCollection.ToList"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CalendarCollection yöntemi. CalendarCollection nesnesini Calendar nesnelerinin bir listesine dönüştürür"
type: docs
weight: 70
url: /tr/net/aspose.tasks/calendarcollection/tolist/
---
## CalendarCollection.ToList method

CalendarCollection nesnesini [`Calendar`](../../calendar/) nesnelerinin bir listesine dönüştürür.

```csharp
public List<Calendar> ToList()
```

### Dönüş Değeri

[`Calendar`](../../calendar/) nesnelerinin listesi.

## Örnekler

Takvim koleksiyonunda nasıl yineleme yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project5.mpp");

Console.WriteLine("Number of calendars in the project: " + project.Calendars.Count);
List<Calendar> calendars = project.Calendars.ToList();
foreach (var calendar in calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Ayrıca Bakınız

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


