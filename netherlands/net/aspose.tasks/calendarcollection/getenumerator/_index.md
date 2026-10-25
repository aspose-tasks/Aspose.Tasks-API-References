---
title: "CalendarCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CalendarCollection-methode. Retourneert een enumerator voor deze collectie."
type: docs
weight: 50
url: /nl/net/aspose.tasks/calendarcollection/getenumerator/
---
## CalendarCollection.GetEnumerator method

Retourneert een enumerator voor deze collectie.

```csharp
public IEnumerator<Calendar> GetEnumerator()
```

### Retourwaarde

een enumerator voor deze collectie.

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


