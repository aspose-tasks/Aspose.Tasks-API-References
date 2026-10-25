---
title: "Duration.Convert"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Duration-methode. Converteert een Duration-object naar een andere duur met opgegeven tijdseenheden"
type: docs
weight: 70
url: /nl/net/aspose.tasks/duration/convert/
---
## Duration.Convert method

Converteert het Duration‑object naar een andere duur met opgegeven tijdseenheden.

```csharp
public Duration Convert(TimeUnitType timeUnitType)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| timeUnitType | TimeUnitType | het opgegeven tijdseenheidtype. |

### Retourwaarde

geeft een nieuwe duur terug met het opgegeven eenheidstype.

## Voorbeelden

Toont hoe een duur kan worden geconverteerd naar verschillende tijdseenheidstypen.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// Verkrijg een taak om de duur in verschillende formaten te berekenen.
var task = project.RootTask.Children.GetById(1);

// Haal de duur op in Minuten, Dagen, Uren, Weken en Maanden.
var mins = task.Get(Tsk.Duration).Convert(TimeUnitType.Minute).ToDouble();
Console.WriteLine("Duration in Mins: {0}", mins);
var days = task.Get(Tsk.Duration).Convert(TimeUnitType.Day).ToDouble();
Console.WriteLine("Duration in Days: {0}", days);
var hours = task.Get(Tsk.Duration).Convert(TimeUnitType.Hour).ToDouble();
Console.WriteLine("Duration in Hours: {0}", hours);
var weeks = task.Get(Tsk.Duration).Convert(TimeUnitType.Week).ToDouble();
Console.WriteLine("Duration in Weeks: {0}", weeks);
var months = task.Get(Tsk.Duration).Convert(TimeUnitType.Month).ToDouble();
Console.WriteLine("Duration in Months: {0}", months);
```

### Zie ook

* enum [TimeUnitType](../../timeunittype/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


