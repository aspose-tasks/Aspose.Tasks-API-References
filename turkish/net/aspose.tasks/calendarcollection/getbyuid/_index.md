---
title: "CalendarCollection.GetByUid"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CalendarCollection yöntemi. Belirtilen UID'ye sahip bir takvim döndürür"
type: docs
weight: 40
url: /tr/net/aspose.tasks/calendarcollection/getbyuid/
---
## CalendarCollection.GetByUid method

Belirtilen UID'ye sahip bir takvimi döndürür.

```csharp
public Calendar GetByUid(int uid)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | Int32 | Bir takvimin UID'si. |

### Dönüş Değeri

Belirtilen UID'ye sahip takvim.

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


