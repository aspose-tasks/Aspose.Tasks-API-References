---
title: "Classe WorkUnit"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.WorkUnit. Rappresenta le ore lavorative"
type: docs
weight: 3630
url: /it/net/aspose.tasks/workunit/
---
## WorkUnit class

Rappresenta le ore lavorative.

```csharp
public class WorkUnit
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [WorkUnit](workunit/)(DateTime, DateTime) | Inizializza una nuova istanza della classe `WorkUnit`. Crea un nuovo oggetto WorkUnit con le date From e To specificate. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [From](../../aspose.tasks/workunit/from/) { get; set; } | Ottiene o imposta la data From. |
| [To](../../aspose.tasks/workunit/to/) { get; set; } | Ottiene o imposta la data To. |
| [WorkingHours](../../aspose.tasks/workunit/workinghours/) { get; set; } | Ottiene o imposta la durata delle ore lavorative. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


