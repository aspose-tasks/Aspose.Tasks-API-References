---
title: "Klasse WorkUnit"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.WorkUnit‑klasse. Vertegenwoordigt werkuren"
type: docs
weight: 3630
url: /nl/net/aspose.tasks/workunit/
---
## WorkUnit class

Stelt werktijden voor.

```csharp
public class WorkUnit
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [WorkUnit](workunit/)(DateTime, DateTime) | Initialiseert een nieuw exemplaar van de `WorkUnit`‑klasse. Creëert een nieuw WorkUnit‑object met de opgegeven From‑ en To‑datums. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [From](../../aspose.tasks/workunit/from/) { get; set; } | Haalt op of stelt de From‑datum in. |
| [To](../../aspose.tasks/workunit/to/) { get; set; } | Haalt op of stelt de To‑datum in. |
| [WorkingHours](../../aspose.tasks/workunit/workinghours/) { get; set; } | Haalt op of stelt de duur van de werkuren in. |

## Voorbeelden

Toont hoe te werken met work‑unit‑informatie.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// haal werkuren op voor een specifieke datum
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

Console.WriteLine("From: " + workUnit.From);
Console.WriteLine("To: " + workUnit.To);
Console.WriteLine("Working hours: " + workUnit.WorkingHours);
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


