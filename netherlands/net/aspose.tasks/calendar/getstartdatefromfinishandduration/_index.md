---
title: "Calendar.GetStartDateFromFinishAndDuration"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Calendar methode. Retourneert de startdatum op basis van de opgegeven einddatum en duur"
type: docs
weight: 200
url: /nl/net/aspose.tasks/calendar/getstartdatefromfinishandduration/
---
## GetStartDateFromFinishAndDuration(DateTime, Duration) {#getstartdatefromfinishandduration}

Retourneert de startdatum op basis van de opgegeven einddatum en duur.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, Duration duration)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| einde | DateTime | De opgegeven einddatum. |
| duur | Duur | De opgegeven duur. |

### Retourwaarde

Berekende startdatum.

## Voorbeelden

Toont hoe een startdatum te krijgen op basis van einddatum en duur.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// get start datum op basis van einddatum en een duur
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), project.GetDuration(16, TimeUnitType.Hour));

// 8 april 2020 9:00 AM wordt afgedrukt
Console.WriteLine(startDate);
```

### Zie ook

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetStartDateFromFinishAndDuration(DateTime, TimeSpan) {#getstartdatefromfinishandduration_1}

Retourneert de startdatum op basis van de opgegeven einddatum en duur.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, TimeSpan duration)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| einde | DateTime | De opgegeven einddatum. |
| duur | TimeSpan | De opgegeven duur. |

### Retourwaarde

Berekende startdatum.

## Voorbeelden

Toont hoe een startdatum te krijgen op basis van einddatum en duur (als een tijdsduur).

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// get start datum op basis van einddatum en een duur
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), TimeSpan.FromHours(16));

// 8 april 2020 9:00 AM wordt afgedrukt
Console.WriteLine(startDate);
```

### Zie ook

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


