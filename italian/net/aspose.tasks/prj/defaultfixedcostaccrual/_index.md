---
title: "Prj.DefaultFixedCostAccrual"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Il tipo predefinito quando i costi fissi sono accumulati"
type: docs
weight: 240
url: /it/net/aspose.tasks/prj/defaultfixedcostaccrual/
---
## Prj.DefaultFixedCostAccrual field

Il tipo predefinito quando i costi fissi sono accumulati.

```csharp
public static readonly Key<CostAccrualType, PrjKey> DefaultFixedCostAccrual;
```

## Esempi

Mostra come leggere le proprietà predefinite del progetto.

```csharp
var project = new Project(DataDir + "DefaultProperties.mpp");

// Imposta le proprietà predefinite
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, DateTime.Now);
project.Set(Prj.DefaultStartTime, project.Get(Prj.StartDate));
project.Set(Prj.DefaultTaskType, TaskType.FixedDuration);
project.Set(Prj.DefaultStandardRate, 15);
project.Set(Prj.DefaultOvertimeRate, 12);
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
project.Set(Prj.DefaultFixedCostAccrual, CostAccrualType.Prorated);

// Visualizza le proprietà predefinite
Console.WriteLine("New Task Default Start: " + project.Get(Prj.DefaultStartTime).ToShortDateString());
Console.WriteLine("New Task Default Type: " + project.Get(Prj.DefaultTaskType));
Console.WriteLine("Resource Default Standard Rate: " + project.Get(Prj.DefaultStandardRate));
Console.WriteLine("Resource Default Overtime Rate: " + project.Get(Prj.DefaultOvertimeRate));
Console.WriteLine("Default Task EV Method: " + project.Get(Prj.DefaultTaskEVMethod));
Console.WriteLine("Default Cost Accrual: " + project.Get(Prj.DefaultFixedCostAccrual));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


