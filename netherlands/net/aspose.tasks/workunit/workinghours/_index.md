---
title: "WorkUnit.WorkingHours"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "WorkUnit-eigenschap. Haalt de duur van de werktijd op of stelt deze in"
type: docs
weight: 40
url: /nl/net/aspose.tasks/workunit/workinghours/
---
## WorkUnit.WorkingHours property

Haalt op of stelt de duur van de werkuren in.

```csharp
public TimeSpan WorkingHours { get; set; }
```

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


