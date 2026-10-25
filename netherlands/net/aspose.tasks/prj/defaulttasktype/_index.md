---
title: "Prj.DefaultTaskType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. Het standaardtype van nieuwe taken"
type: docs
weight: 290
url: /nl/net/aspose.tasks/prj/defaulttasktype/
---
## Prj.DefaultTaskType field

Het standaardtype van nieuwe taken.

```csharp
public static readonly Key<TaskType, PrjKey> DefaultTaskType;
```

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

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskType](../../tasktype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


