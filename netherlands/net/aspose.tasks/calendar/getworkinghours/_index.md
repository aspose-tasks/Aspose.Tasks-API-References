---
title: "Calendar.GetWorkingHours"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Calendar-methode. Retourneert WorkUnit, Start, Finish en Duur van werktijden voor het opgegeven datum‑tijdinterval"
type: docs
weight: 220
url: /nl/net/aspose.tasks/calendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

Retourneer WorkUnit - Start, Eind en Duur van werktijden voor het opgegeven datum‑tijdinterval.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | DateTime | Startdatum van het interval. |
| einde | DateTime | Einddatum van het interval. |

### Retourwaarde

Instantie van de [`WorkUnit`](../../workunit/) klasse die Start, Finish en Duration van werktijd bevat.

## Voorbeelden

Toont hoe werktijden voor specifieke data op te halen.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// haal werkuren op voor een specifieke datum
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

// 16 uur zullen worden afgedrukt
Console.WriteLine(workUnit.WorkingHours);
```

### Zie ook

* class [WorkUnit](../../workunit/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

Retourneert het aantal werkuren op de opgegeven datum.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dt | DateTime | De datum om werktijden voor op te halen. |

### Retourwaarde

Werktijden op de opgegeven datum.

## Voorbeelden

Toont hoe werktijden voor een specifieke datum op te halen.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// haal werkuren op voor een specifieke datum
var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 10));

// 8 uur zal worden afgedrukt
Console.WriteLine(workingHours.Hours);
```

### Zie ook

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


