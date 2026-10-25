---
title: "Prj.FinishDate"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. De einddatum van een project"
type: docs
weight: 330
url: /nl/net/aspose.tasks/prj/finishdate/
---
## Prj.FinishDate field

De einddatum van een project.

```csharp
public static readonly Key<DateTime, PrjKey> FinishDate;
```

## Voorbeelden

Toont hoe het project opnieuw te plannen vanaf de einddatum in plaats van de startdatum.

```csharp
var project = new Project();
project.Set(Prj.ScheduleFromStart, false);
project.Set(Prj.FinishDate, new DateTime(2020, 1, 1));

// Nu worden alle taakdatums (Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish) berekend. Om het kritieke pad te verkrijgen moeten we de speling berekenen (kan worden aangeroepen in een aparte thread, maar alleen na de berekening van alle vroege/late datums).
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


