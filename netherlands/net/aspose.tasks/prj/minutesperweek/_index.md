---
title: "Prj.MinutesPerWeek"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. Het aantal minuten per week"
type: docs
weight: 480
url: /nl/net/aspose.tasks/prj/minutesperweek/
---
## Prj.MinutesPerWeek field

Het aantal minuten per week.

```csharp
public static readonly Key<int, PrjKey> MinutesPerWeek;
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
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


