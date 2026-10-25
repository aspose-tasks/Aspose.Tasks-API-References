---
title: "WorkUnit.From"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "WorkUnit-eigenschap. Haalt de From-datum op of stelt deze in"
type: docs
weight: 20
url: /nl/net/aspose.tasks/workunit/from/
---
## WorkUnit.From property

Haalt op of stelt de From‑datum in.

```csharp
public DateTime From { get; set; }
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


