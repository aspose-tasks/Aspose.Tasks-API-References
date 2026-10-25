---
title: "WorkUnit.From"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà WorkUnit. Ottiene o imposta la data From"
type: docs
weight: 20
url: /it/net/aspose.tasks/workunit/from/
---
## WorkUnit.From property

Ottiene o imposta la data From.

```csharp
public DateTime From { get; set; }
```

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


