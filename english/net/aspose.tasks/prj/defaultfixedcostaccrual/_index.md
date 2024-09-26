---
title: Prj.DefaultFixedCostAccrual
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The default type when fixed costs are accrued
type: docs
weight: 240
url: /net/aspose.tasks/prj/defaultfixedcostaccrual/
---
## Prj.DefaultFixedCostAccrual field

The default type when fixed costs are accrued.

```csharp
public static readonly Key<CostAccrualType, PrjKey> DefaultFixedCostAccrual;
```

## Examples

Shows how to read project's default properties.

```csharp
var project = new Project(DataDir + "DefaultProperties.mpp");

// Set default properties
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, DateTime.Now);
project.Set(Prj.DefaultStartTime, project.Get(Prj.StartDate));
project.Set(Prj.DefaultTaskType, TaskType.FixedDuration);
project.Set(Prj.DefaultStandardRate, 15);
project.Set(Prj.DefaultOvertimeRate, 12);
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
project.Set(Prj.DefaultFixedCostAccrual, CostAccrualType.Prorated);

// Display default properties
Console.WriteLine("New Task Default Start: " + project.Get(Prj.DefaultStartTime).ToShortDateString());
Console.WriteLine("New Task Default Type: " + project.Get(Prj.DefaultTaskType));
Console.WriteLine("Resource Default Standard Rate: " + project.Get(Prj.DefaultStandardRate));
Console.WriteLine("Resource Default Overtime Rate: " + project.Get(Prj.DefaultOvertimeRate));
Console.WriteLine("Default Task EV Method: " + project.Get(Prj.DefaultTaskEVMethod));
Console.WriteLine("Default Cost Accrual: " + project.Get(Prj.DefaultFixedCostAccrual));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


