---
title: "Prj.WeekStartDay"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. Eerste dag van een week"
type: docs
weight: 780
url: /nl/net/aspose.tasks/prj/weekstartday/
---
## Prj.WeekStartDay field

Eerste dag van een week.

```csharp
public static readonly Key<DayType, PrjKey> WeekStartDay;
```

## Voorbeelden

Toont hoe de weekdag-eigenschappen van een project te lezen/schrijven.

```csharp
var project = new Project(DataDir + "WriteWeekdayProperties.mpp");

// Stel weekdag-eigenschappen in
project.Set(Prj.WeekStartDay, DayType.Monday);
project.Set(Prj.DaysPerMonth, 24);
project.Set(Prj.MinutesPerDay, 540);
project.Set(Prj.MinutesPerWeek, 3240);

// Toon weekdag-eigenschappen
Console.WriteLine("Week Start Date: " + project.Get(Prj.WeekStartDay));
Console.WriteLine("Days Per Month: " + project.Get(Prj.DaysPerMonth));
Console.WriteLine("Minutes Per Day: " + project.Get(Prj.MinutesPerDay));
Console.WriteLine("Minutes Per Week: " + project.Get(Prj.MinutesPerWeek));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [DayType](../../daytype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


