---
title: Class WorkUnit
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.WorkUnit class. Represents working hours
type: docs
weight: 3610
url: /net/aspose.tasks/workunit/
---
## WorkUnit class

Represents working hours.

```csharp
public class WorkUnit
```

## Constructors

| Name | Description |
| --- | --- |
| [WorkUnit](workunit/)(DateTime, DateTime) | Initializes a new instance of the `WorkUnit` class. Creates new WorkUnit object with the specified From and To dates. |

## Properties

| Name | Description |
| --- | --- |
| [From](../../aspose.tasks/workunit/from/) { get; set; } | Gets or sets the From date. |
| [To](../../aspose.tasks/workunit/to/) { get; set; } | Gets or sets the To date. |
| [WorkingHours](../../aspose.tasks/workunit/workinghours/) { get; set; } | Gets or sets the duration of working hours. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


