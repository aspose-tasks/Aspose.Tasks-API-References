---
title: "Calendar.Uid"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Calendar property. Ottiene o imposta l'identificatore univoco del calendario"
type: docs
weight: 110
url: /it/net/aspose.tasks/calendar/uid/
---
## Calendar.Uid property

Ottiene o imposta l'identificatore univoco del calendario.

```csharp
public int Uid { get; set; }
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


