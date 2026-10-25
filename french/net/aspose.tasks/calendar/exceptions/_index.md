---
title: "Calendar.Exceptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Calendar. Obtient l'objet CalendarExceptionCollection. La collection d'exceptions associée au calendrier"
type: docs
weight: 50
url: /fr/net/aspose.tasks/calendar/exceptions/
---
## Calendar.Exceptions property

Obtient l'objet CalendarExceptionCollection. La collection d'exceptions associée au calendrier.

```csharp
public CalendarExceptionCollection Exceptions { get; }
```

## Exemples

Montre comment récupérer les informations sur les exceptions du calendrier.

```csharp
var project = new Project(DataDir + "project_RetrieveExceptions_test.mpp");

// Itérer sur les calendriers
foreach (var calendar in project.Calendars)
{
    // Accéder aux exceptions du calendrier
    foreach (var exception in calendar.Exceptions)
    {
        Console.WriteLine("From: " + exception.FromDate.ToShortDateString());
        Console.WriteLine("To: " + exception.ToDate.ToShortDateString());
    }
}
```

### Voir aussi

* class [CalendarExceptionCollection](../../calendarexceptioncollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


