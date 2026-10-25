---
title: "Classe WorkUnit"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.WorkUnit. Représente les heures de travail"
type: docs
weight: 3630
url: /fr/net/aspose.tasks/workunit/
---
## WorkUnit class

Représente les heures de travail.

```csharp
public class WorkUnit
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [WorkUnit](workunit/)(DateTime, DateTime) | Initialise une nouvelle instance de la classe `WorkUnit`. Crée un nouvel objet WorkUnit avec les dates From et To spécifiées. |

## Propriétés

| Nom | Description |
| --- | --- |
| [From](../../aspose.tasks/workunit/from/) { get; set; } | Obtient ou définit la date From. |
| [To](../../aspose.tasks/workunit/to/) { get; set; } | Obtient ou définit la date To. |
| [WorkingHours](../../aspose.tasks/workunit/workinghours/) { get; set; } | Obtient ou définit la durée des heures de travail. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


