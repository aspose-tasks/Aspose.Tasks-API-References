---
title: Prj.DaysPerMonth
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The number of days per month
type: docs
weight: 220
url: /net/aspose.tasks/prj/dayspermonth/
---
## Prj.DaysPerMonth field

The number of days per month.

```csharp
public static readonly Key<int, PrjKey> DaysPerMonth;
```

## Examples

Shows how to read/write project's weekday properties.

```csharp
var project = new Project(DataDir + "WriteWeekdayProperties.mpp");

// Set week days properties
project.Set(Prj.WeekStartDay, DayType.Monday);
project.Set(Prj.DaysPerMonth, 24);
project.Set(Prj.MinutesPerDay, 540);
project.Set(Prj.MinutesPerWeek, 3240);

// Display week days properties
Console.WriteLine("Week Start Date: " + project.Get(Prj.WeekStartDay));
Console.WriteLine("Days Per Month: " + project.Get(Prj.DaysPerMonth));
Console.WriteLine("Minutes Per Day: " + project.Get(Prj.MinutesPerDay));
Console.WriteLine("Minutes Per Week: " + project.Get(Prj.MinutesPerWeek));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


