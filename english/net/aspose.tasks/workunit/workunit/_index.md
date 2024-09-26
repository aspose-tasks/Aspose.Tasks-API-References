---
title: WorkUnit.WorkUnit
second_title: Aspose.Tasks for .NET API Reference
description: WorkUnit constructor. Initializes a new instance of the WorkUnit class. Creates new WorkUnit object with the specified From and To dates
type: docs
weight: 10
url: /net/aspose.tasks/workunit/workunit/
---
## WorkUnit constructor

Initializes a new instance of the [`WorkUnit`](../) class. Creates new WorkUnit object with the specified From and To dates.

```csharp
public WorkUnit(DateTime from, DateTime to)
```

| Parameter | Type | Description |
| --- | --- | --- |
| from | DateTime | Start date of working hours. |
| to | DateTime | Finish date of working hours. |

## Examples

Shows how to work with work unit information.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// get working hours for specific date
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

Console.WriteLine("From: " + workUnit.From);
Console.WriteLine("To: " + workUnit.To);
Console.WriteLine("Working hours: " + workUnit.WorkingHours);
```

### See Also

* class [WorkUnit](../)
* namespace [Aspose.Tasks](../../workunit/)
* assembly [Aspose.Tasks](../../../)


