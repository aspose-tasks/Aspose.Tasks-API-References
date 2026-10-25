---
title: "CalendarCollection.Add"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CalendarCollection methode. Voegt een nieuwe basisagenda toe aan dit CalendarCollection-object en retourneert de toegevoegde agenda."
type: docs
weight: 20
url: /nl/net/aspose.tasks/calendarcollection/add/
---
## Add(string) {#add}

Voegt een nieuwe basis‑Calendar toe aan dit CalendarCollection-object en retourneert de toegevoegde Calendar.

```csharp
public Calendar Add(string name)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | Naam van de agenda. |

### Retourwaarde

Toegevoegd [`Calendar`](../../calendar/) object.

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| ArgumentException | Wordt gegooid wanneer de agendanaam null is. |

## Voorbeelden

Toont hoe een standaardagenda te maken.

```csharp
var project = new Project();

// Definieer een agenda en maak deze standaard.
var calendar = project.Calendars.Add("New Standard Calendar");
Calendar.MakeStandardCalendar(calendar);

project.Save(OutDir + "MakeAStandardCalendar_out.xml", SaveFileFormat.Xml);
```

### Zie ook

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, Calendar) {#add_1}

Voegt een nieuwe Calendar toe met de opgegeven basis‑Calendar aan dit CalendarCollection-object en retourneert de toegevoegde Calendar.

```csharp
public Calendar Add(string name, Calendar baseCalendar)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | Opgegeven naam. |
| baseCalendar | Calendar | Opgegeven basisagenda. |

### Retourwaarde

Toegevoegd [`Calendar`](../../calendar/) object.

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

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


