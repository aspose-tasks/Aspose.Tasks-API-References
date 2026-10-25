---
title: "Calendar.GetNextWorkingDayStart"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Calendar-methode. Berekent het begin van de volgende werkdag voor de opgegeven datum"
type: docs
weight: 180
url: /nl/net/aspose.tasks/calendar/getnextworkingdaystart/
---
## Calendar.GetNextWorkingDayStart method

Berekent het begin van de volgende werkdag voor de opgegeven datum.

```csharp
public DateTime GetNextWorkingDayStart(DateTime date)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| datum | DateTime | De datum waarvoor het begin van de volgende werkdag moet worden opgehaald. |

### Retourwaarde

Begin van de volgende werkdag DateTime.

## Voorbeelden

Toont hoe het begin van de volgende werkdag te verkrijgen met behulp van een kalender.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// verkrijg het begin van de volgende werkdag (weekend wordt overgeslagen)
var nextWorkingDayStart = calendar.GetNextWorkingDayStart(new DateTime(2020, 4, 10, 13, 0, 0));

// 13 april 2020 9:00 AM wordt afgedrukt
Console.WriteLine(nextWorkingDayStart);
```

### Zie ook

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


