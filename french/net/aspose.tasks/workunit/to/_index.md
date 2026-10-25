---
title: "WorkUnit.To"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété WorkUnit. Obtient ou définit la date To"
type: docs
weight: 30
url: /fr/net/aspose.tasks/workunit/to/
---
## WorkUnit.To property

Obtient ou définit la date To.

```csharp
public DateTime To { get; set; }
```

## Exemples

Montre comment travailler avec les informations d'unité de travail.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// obtenez les heures de travail pour une date spécifique
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

Console.WriteLine("From: " + workUnit.From);
Console.WriteLine("To: " + workUnit.To);
Console.WriteLine("Working hours: " + workUnit.WorkingHours);
```

### Voir aussi

* class [WorkUnit](../)
* namespace [Aspose.Tasks](../../workunit/)
* assembly [Aspose.Tasks](../../../)


