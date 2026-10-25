---
title: "Klasse CalendarCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.CalendarCollection klasse. Vertegenwoordigt een verzameling van Calendar-objecten."
type: docs
weight: 240
url: /nl/net/aspose.tasks/calendarcollection/
---
## CalendarCollection class

Vertegenwoordigt een verzameling van [`Calendar`](../calendar/) objecten.

```csharp
public class CalendarCollection : IList<Calendar>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/calendarcollection/count/) { get; } | Haalt het aantal objecten op dat in dit `CalendarCollection` object zit. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/calendarcollection/add/#add)(string) | Voegt een nieuwe basis‑Calendar toe aan dit CalendarCollection-object en retourneert de toegevoegde Calendar. |
| [Add](../../aspose.tasks/calendarcollection/add/#add_1)(string, Calendar) | Voegt een nieuwe Calendar toe met de opgegeven basis‑Calendar aan dit CalendarCollection-object en retourneert de toegevoegde Calendar. |
| [GetByName](../../aspose.tasks/calendarcollection/getbyname/)(string) | Retourneert een Calendar met de opgegeven naam. |
| [GetByUid](../../aspose.tasks/calendarcollection/getbyuid/)(int) | Retourneert een Calendar met de opgegeven UID. |
| [GetEnumerator](../../aspose.tasks/calendarcollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [Remove](../../aspose.tasks/calendarcollection/remove/)(Calendar) | Verwijdert Calendar uit de Project CalendarCollection. |
| [ToList](../../aspose.tasks/calendarcollection/tolist/)() | Converteert het CalendarCollection-object naar een lijst van [`Calendar`](../calendar/) objecten. |

## Voorbeelden

Toont hoe nieuwe calendars toe te voegen.

```csharp
var project = new Project();

// Nieuwe calendars kunnen aan de calendar‑verzameling van een project worden toegevoegd door de Add‑overloads van de verzameling te gebruiken.
project.Calendars.Add("Calendar");
var newCalendar = project.Calendars.Add("Parent");
project.Calendars.Add("Child", newCalendar);

foreach (var calendar in project.Calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Zie ook

* class [Calendar](../calendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


