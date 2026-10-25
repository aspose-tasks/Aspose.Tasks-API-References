---
title: "Prj.ScheduleFromStart"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. Bepaalt of het projectschema moet worden berekend vanaf de startdatum"
type: docs
weight: 630
url: /nl/net/aspose.tasks/prj/schedulefromstart/
---
## Prj.ScheduleFromStart field

Bepaalt of het projectschema vooruit moet worden berekend vanaf de startdatum.

```csharp
public static readonly Key<NullableBool, PrjKey> ScheduleFromStart;
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
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


