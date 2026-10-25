---
title: "Calendar.Exceptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Calendar özelliği. CalendarExceptionCollection nesnesini alır. Takvimle ilişkili istisnaların koleksiyonu."
type: docs
weight: 50
url: /tr/net/aspose.tasks/calendar/exceptions/
---
## Calendar.Exceptions property

CalendarExceptionCollection nesnesini alır. Takvimle ilişkili istisna koleksiyonunu içerir.

```csharp
public CalendarExceptionCollection Exceptions { get; }
```

## Örnekler

Takvim istisnaları hakkında bilgi almanın nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "project_RetrieveExceptions_test.mpp");

// Takvimler üzerinde yineleme yapın
foreach (var calendar in project.Calendars)
{
    // Takvim istisnalarına erişin
    foreach (var exception in calendar.Exceptions)
    {
        Console.WriteLine("From: " + exception.FromDate.ToShortDateString());
        Console.WriteLine("To: " + exception.ToDate.ToShortDateString());
    }
}
```

### Ayrıca Bakınız

* class [CalendarExceptionCollection](../../calendarexceptioncollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


