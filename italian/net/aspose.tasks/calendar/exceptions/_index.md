---
title: "Calendar.Exceptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Calendar. Ottiene l'oggetto CalendarExceptionCollection. La raccolta di eccezioni associata al calendario"
type: docs
weight: 50
url: /it/net/aspose.tasks/calendar/exceptions/
---
## Calendar.Exceptions property

Ottiene l'oggetto CalendarExceptionCollection. La raccolta di eccezioni associata al calendario.

```csharp
public CalendarExceptionCollection Exceptions { get; }
```

## Esempi

Mostra come recuperare le informazioni sulle eccezioni del calendario.

```csharp
var project = new Project(DataDir + "project_RetrieveExceptions_test.mpp");

// Itera sui calendari
foreach (var calendar in project.Calendars)
{
    // Accedi alle eccezioni del calendario
    foreach (var exception in calendar.Exceptions)
    {
        Console.WriteLine("From: " + exception.FromDate.ToShortDateString());
        Console.WriteLine("To: " + exception.ToDate.ToShortDateString());
    }
}
```

### Vedi anche

* class [CalendarExceptionCollection](../../calendarexceptioncollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


