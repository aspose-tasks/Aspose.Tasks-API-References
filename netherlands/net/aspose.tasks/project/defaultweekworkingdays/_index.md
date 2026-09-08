---
title: "Project.DefaultWeekWorkingDays"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project-eigenschap. Haalt de instantie van de WeekDayCollection-klasse op die een verzameling van de standaard weekwerkdagen en werktijden van het project vertegenwoordigt"
type: docs
weight: 370
url: /nl/net/aspose.tasks/project/defaultweekworkingdays/
---
## Project.DefaultWeekWorkingDays property

Haalt de instantie van de [`WeekDayCollection`](../../weekdaycollection/) klasse op die een verzameling van de standaard weekwerkdagen en werktijden van het project vertegenwoordigt.

```csharp
public WeekDayCollection DefaultWeekWorkingDays { get; }
```

### Retourwaarde

De instantie van de [`WeekDayCollection`](../../weekdaycollection/) klasse die een lijst van [`WeekDay`](../../weekday/) objecten bevat.

## Opmerkingen

De gegevens komen alleen voor in mpp-bestanden (niet in xml).

## Voorbeelden

Toont hoe de standaard weekwerkdag op te halen.

```csharp
var project = new Project(DataDir + "Project2003.mpp");
foreach (var weekDay in project.DefaultWeekWorkingDays)
{
    Console.WriteLine("From: " + weekDay.FromDate);
    Console.WriteLine("From: " + weekDay.ToDate);
    Console.WriteLine("Day type: " + weekDay.DayType);
    Console.WriteLine("Is day working: " + weekDay.DayWorking);
}
```

### Zie ook

* class [WeekDayCollection](../../weekdaycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


