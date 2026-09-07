---
title: "Prj.MinutesPerWeek"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Ο αριθμός των λεπτών ανά εβδομάδα"
type: docs
weight: 480
url: /el/net/aspose.tasks/prj/minutesperweek/
---
## Prj.MinutesPerWeek field

Ο αριθμός των λεπτών ανά εβδομάδα.

```csharp
public static readonly Key<int, PrjKey> MinutesPerWeek;
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


