---
title: "Enum TaskType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.TaskType enum. Specificeert het type van een taak"
type: docs
weight: 2470
url: /nl/net/aspose.tasks/tasktype/
---
## TaskType enumeration

Specificeert het type van een taak.

```csharp
public enum TaskType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Undefined | `-1` | Een ongedefinieerde waarde betekent dat het veld niet is gedefinieerd in het originele bestand |
| FixedUnits | `0` | Vaste eenheden |
| FixedDuration | `1` | Vaste duur |
| FixedWork | `2` | Vast werk |

## Opmerkingen

Tijdens het exporteren naar XML worden de Undefined‑waarden uit de resulterende XML verwijderd.

## Voorbeelden

Toont hoe de standaardeigenschappen van het project te lezen.

```csharp
var project = new Project(DataDir + "DefaultProperties.mpp");

// Standaardeigenschappen instellen
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, DateTime.Now);
project.Set(Prj.DefaultStartTime, project.Get(Prj.StartDate));
project.Set(Prj.DefaultTaskType, TaskType.FixedDuration);
project.Set(Prj.DefaultStandardRate, 15);
project.Set(Prj.DefaultOvertimeRate, 12);
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
project.Set(Prj.DefaultFixedCostAccrual, CostAccrualType.Prorated);

// Standaardeigenschappen weergeven
Console.WriteLine("New Task Default Start: " + project.Get(Prj.DefaultStartTime).ToShortDateString());
Console.WriteLine("New Task Default Type: " + project.Get(Prj.DefaultTaskType));
Console.WriteLine("Resource Default Standard Rate: " + project.Get(Prj.DefaultStandardRate));
Console.WriteLine("Resource Default Overtime Rate: " + project.Get(Prj.DefaultOvertimeRate));
Console.WriteLine("Default Task EV Method: " + project.Get(Prj.DefaultTaskEVMethod));
Console.WriteLine("Default Cost Accrual: " + project.Get(Prj.DefaultFixedCostAccrual));
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


