---
title: "Calendar.BaseCalendar"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Calendar. Ottiene o imposta il calendario base da cui dipende questo calendario. Applicabile solo se il calendario non è un calendario base"
type: docs
weight: 40
url: /it/net/aspose.tasks/calendar/basecalendar/
---
## Calendar.BaseCalendar property

Ottiene o imposta il calendario base da cui dipende questo calendario. Applicabile solo se il calendario non è un calendario base.

```csharp
public Calendar BaseCalendar { get; set; }
```

## Esempi

Mostra come lavorare con un calendario base del calendario della risorsa.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var resource = project.Resources.Add("Resource1");

// Aggiungi calendario standard e assegnalo alla risorsa
var calendar = project.Calendars.Add("Resource1");
resource.Set(Rsc.Calendar, calendar);

// Visualizza il nome del calendario base per tutte le risorse
foreach (var rsc in project.Resources)
{
    if (rsc.Get(Rsc.Name) != null)
    {
        Console.WriteLine(rsc.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### Vedi anche

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


