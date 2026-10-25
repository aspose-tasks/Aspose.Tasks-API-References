---
title: "WorkUnit.WorkUnit"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore WorkUnit. Inizializza una nuova istanza della classe WorkUnit. Crea un nuovo oggetto WorkUnit con le date From e To specificate."
type: docs
weight: 10
url: /it/net/aspose.tasks/workunit/workunit/
---
## WorkUnit constructor

Inizializza una nuova istanza della classe [`WorkUnit`](../). Crea un nuovo oggetto WorkUnit con le date From e To specificate.

```csharp
public WorkUnit(DateTime from, DateTime to)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| da | DateTime | Data di inizio dell'orario di lavoro. |
| a | DateTime | Data di fine dell'orario di lavoro. |

## Esempi

Mostra come lavorare con le informazioni dell'unità di lavoro.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// ottieni le ore lavorative per una data specifica
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

Console.WriteLine("From: " + workUnit.From);
Console.WriteLine("To: " + workUnit.To);
Console.WriteLine("Working hours: " + workUnit.WorkingHours);
```

### Vedi anche

* class [WorkUnit](../)
* namespace [Aspose.Tasks](../../workunit/)
* assembly [Aspose.Tasks](../../../)


