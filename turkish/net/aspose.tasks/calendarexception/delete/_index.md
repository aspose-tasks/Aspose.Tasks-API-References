---
title: "CalendarException.Delete"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CalendarException yöntemi. Exception örneğini üst takvim CalendarExceptionCollection nesnesinden siler"
type: docs
weight: 180
url: /tr/net/aspose.tasks/calendarexception/delete/
---
## CalendarException.Delete method

Exception örneğini üst takvim CalendarExceptionCollection nesnesinden siler.

```csharp
public void Delete()
```

## Örnekler

Bir takvim istisnasının nasıl silineceğini gösterir.

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);

// İstisnayı kaldır
calendar.Exceptions[0].Delete();

Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
```

### Ayrıca Bakınız

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


