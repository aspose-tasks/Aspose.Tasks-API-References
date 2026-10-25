---
title: "Calendar.GetFinishDateByStartAndWork"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Calendar-methode. Berekent de datum waarop de opgegeven hoeveelheid werktijd is verstreken volgens de calendar"
type: docs
weight: 160
url: /nl/net/aspose.tasks/calendar/getfinishdatebystartandwork/
---
## GetFinishDateByStartAndWork(DateTime, Duration) {#getfinishdatebystartandwork}

Berekent de datum waarop de opgegeven hoeveelheid werktijd volgens de kalender zal verstrijken.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, Duration work)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | DateTime | Startdatum. |
| werk | Duur | Werkduur. |

### Retourwaarde

Einddatum.

## Voorbeelden

Toont hoe een einddatum te berekenen op basis van startdatum en werk met een calendar instance.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// bereken einddatum met een standaard calendar
var finish = calendar.GetFinishDateByStartAndWork(start, work);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### Zie ook

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetFinishDateByStartAndWork(DateTime, TimeSpan) {#getfinishdatebystartandwork_1}

Berekent de datum waarop de opgegeven hoeveelheid werktijd volgens de kalender zal verstrijken.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, TimeSpan work)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | DateTime | Startdatum. |
| werk | TimeSpan | Werkduur. |

### Retourwaarde

Einddatum.

## Voorbeelden

Toont hoe een einddatum te berekenen op basis van startdatum en werk (als tijdsduur) met een calendar instance.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// bereken einddatum met een standaard calendar
var finish = calendar.GetFinishDateByStartAndWork(start, work.TimeSpan);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### Zie ook

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


