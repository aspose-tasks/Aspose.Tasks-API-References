---
title: "Prj.DefaultTaskEVMethod"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj veld. De standaard verdiende-waarde methode voor taken"
type: docs
weight: 280
url: /nl/net/aspose.tasks/prj/defaulttaskevmethod/
---
## Prj.DefaultTaskEVMethod field

De standaardmethode voor verdiende waarde voor taken.

```csharp
public static readonly Key<EarnedValueMethodType, PrjKey> DefaultTaskEVMethod;
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
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


