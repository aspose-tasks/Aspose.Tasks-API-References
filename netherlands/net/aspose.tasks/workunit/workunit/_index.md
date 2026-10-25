---
title: "WorkUnit.WorkUnit"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "WorkUnit constructor. Initialiseert een nieuw exemplaar van de WorkUnit-klasse. Maakt een nieuw WorkUnit-object aan met de opgegeven From- en To-datums"
type: docs
weight: 10
url: /nl/net/aspose.tasks/workunit/workunit/
---
## WorkUnit constructor

Initialiseert een nieuw exemplaar van de [`WorkUnit`](../) klasse. Maakt een nieuw WorkUnit-object aan met de opgegeven From- en To-datums.

```csharp
public WorkUnit(DateTime from, DateTime to)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| van | DateTime | Startdatum van de werktijd. |
| naar | DateTime | Einddatum van de werktijd. |

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

* class [WorkUnit](../)
* namespace [Aspose.Tasks](../../workunit/)
* assembly [Aspose.Tasks](../../../)


