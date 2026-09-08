---
title: "Calendar.GetWorkingTimes"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Calendar-methode. Retourneert WorkingTimeCollection van werktijden voor de opgegeven datum"
type: docs
weight: 240
url: /nl/net/aspose.tasks/calendar/getworkingtimes/
---
## Calendar.GetWorkingTimes method

Retourneert [`WorkingTimeCollection`](../../workingtimecollection/) van werktijden voor de opgegeven datum.

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dt | DateTime | De datum om werktijden voor op te halen. |

### Retourwaarde

Collectie van [`WorkingTime`](../../workingtime/) instanties.

## Voorbeelden

Toont hoe werktijden voor een specifieke datum op te halen.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// haal werktijden op voor specifieke datum
var workingTimes = calendar.GetWorkingTimes(new DateTime(2020, 4, 8, 8, 0, 0));

// 16 uur zullen worden afgedrukt
foreach (var workingTime in workingTimes)
{
    Console.WriteLine("From: " + workingTime.From);
    Console.WriteLine("To: " + workingTime.To);
}
```

### Zie ook

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


