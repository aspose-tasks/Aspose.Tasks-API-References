---
title: "Prj.MinutesPerWeek"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Prj field. Il numero di minuti per settimana"
type: docs
weight: 480
url: /it/net/aspose.tasks/prj/minutesperweek/
---
## Prj.MinutesPerWeek field

Il numero di minuti alla settimana.

```csharp
public static readonly Key<int, PrjKey> MinutesPerWeek;
```

## Esempi

Mostra come leggere/scrivere le proprietà dei giorni feriali del progetto.

```csharp
var project = new Project(DataDir + "WriteWeekdayProperties.mpp");

// Imposta le proprietà dei giorni feriali
project.Set(Prj.WeekStartDay, DayType.Monday);
project.Set(Prj.DaysPerMonth, 24);
project.Set(Prj.MinutesPerDay, 540);
project.Set(Prj.MinutesPerWeek, 3240);

// Visualizza le proprietà dei giorni feriali
Console.WriteLine("Week Start Date: " + project.Get(Prj.WeekStartDay));
Console.WriteLine("Days Per Month: " + project.Get(Prj.DaysPerMonth));
Console.WriteLine("Minutes Per Day: " + project.Get(Prj.MinutesPerDay));
Console.WriteLine("Minutes Per Week: " + project.Get(Prj.MinutesPerWeek));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


