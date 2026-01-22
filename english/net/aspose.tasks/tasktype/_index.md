---
title: Enum TaskType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TaskType enum. Specifies the type of a task
type: docs
weight: 2440
url: /net/aspose.tasks/tasktype/
---
## TaskType enumeration

Specifies the type of a task.

```csharp
public enum TaskType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Undefined | `-1` | Undefined value means that the field was not defined in original file |
| FixedUnits | `0` | Fixed units |
| FixedDuration | `1` | Fixed duration |
| FixedWork | `2` | Fixed work |

## Remarks

While exporting into XML the Undefined values will be eliminated from resulting XML.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


