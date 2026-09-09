---
title: "CalendarCollection.GetByName"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CalendarCollection yöntemi. Belirtilen ada sahip bir takvimi döndürür."
type: docs
weight: 30
url: /tr/net/aspose.tasks/calendarcollection/getbyname/
---
## CalendarCollection.GetByName method

Belirtilen ada sahip bir takvimi döndürür.

```csharp
public Calendar GetByName(string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | Dize | Bir takvimin adı. |

### Dönüş Değeri

Bulunursa belirtilen ada sahip takvimi döndürür, aksi takdirde null döndürür.

## Örnekler

Takvimleri ada veya kimliğe göre nasıl alacağınızı gösterir.

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendarByName = project.Calendars.GetByName("TestCalendar");
var calendarByUid = project.Calendars.GetByUid(4);

Console.WriteLine("Calendar Name: " + calendarByName.Name);
Console.WriteLine("Calendar Name: " + calendarByUid.Name);
Console.WriteLine("Are calendars equals: " + calendarByName.Equals(calendarByUid));
```

### Ayrıca Bakınız

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


