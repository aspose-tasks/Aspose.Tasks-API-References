---
title: "Calendar.GetPreviousWorkingDayEnd"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Kalender-methode. Berekent het einde van de vorige werkdag vanaf de opgegeven datum"
type: docs
weight: 190
url: /nl/net/aspose.tasks/calendar/getpreviousworkingdayend/
---
## Calendar.GetPreviousWorkingDayEnd method

Berekent het einde van de vorige werkdag vanaf de opgegeven datum.

```csharp
public DateTime GetPreviousWorkingDayEnd(DateTime date)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| datum | DateTime | de datum om het einde van de vorige werkdag te berekenen. |

### Retourwaarde

Het einde van de vorige werkdag.

## Voorbeelden

Toont hoe het einde van een vorige werkdag te verkrijgen met behulp van een kalender.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// verkrijg einde van vorige werkdag
var previousWorkingDayEnd = calendar.GetPreviousWorkingDayEnd(new DateTime(2020, 4, 10, 13, 0, 0));

// 9 april 2020 18:00 uur wordt afgedrukt
Console.WriteLine(previousWorkingDayEnd);
```

### Zie ook

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


