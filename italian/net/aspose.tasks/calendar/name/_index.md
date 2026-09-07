---
title: "Calendar.Name"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Calendar. Ottiene o imposta il nome del calendario"
type: docs
weight: 90
url: /it/net/aspose.tasks/calendar/name/
---
## Calendar.Name property

Ottiene o imposta il nome del calendario.

```csharp
public string Name { get; set; }
```

## Esempi

Mostra come recuperare le informazioni del calendario.

```csharp
var project = new Project(DataDir + "RetrieveCalendarInfo.mpp");

// Recupera le informazioni dei calendari
foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("Calendar UID: " + calendar.Uid);
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Vedi anche

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


