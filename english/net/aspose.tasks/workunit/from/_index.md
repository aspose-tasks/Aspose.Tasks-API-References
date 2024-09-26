---
title: WorkUnit.From
second_title: Aspose.Tasks for .NET API Reference
description: WorkUnit property. Gets or sets the From date
type: docs
weight: 20
url: /net/aspose.tasks/workunit/from/
---
## WorkUnit.From property

Gets or sets the From date.

```csharp
public DateTime From { get; set; }
```

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


