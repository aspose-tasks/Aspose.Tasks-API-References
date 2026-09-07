---
title: "Prj.DaysPerMonth"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Ο αριθμός ημερών ανά μήνα"
type: docs
weight: 220
url: /el/net/aspose.tasks/prj/dayspermonth/
---
## Prj.DaysPerMonth field

Ο αριθμός ημερών ανά μήνα.

```csharp
public static readonly Key<int, PrjKey> DaysPerMonth;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε τις ιδιότητες των εργάσιμων ημερών του έργου.

```csharp
var project = new Project(DataDir + "WriteWeekdayProperties.mpp");

// Ορίστε τις ιδιότητες των εργάσιμων ημερών
project.Set(Prj.WeekStartDay, DayType.Monday);
project.Set(Prj.DaysPerMonth, 24);
project.Set(Prj.MinutesPerDay, 540);
project.Set(Prj.MinutesPerWeek, 3240);

// Εμφανίστε τις ιδιότητες των εργάσιμων ημερών
Console.WriteLine("Week Start Date: " + project.Get(Prj.WeekStartDay));
Console.WriteLine("Days Per Month: " + project.Get(Prj.DaysPerMonth));
Console.WriteLine("Minutes Per Day: " + project.Get(Prj.MinutesPerDay));
Console.WriteLine("Minutes Per Week: " + project.Get(Prj.MinutesPerWeek));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


