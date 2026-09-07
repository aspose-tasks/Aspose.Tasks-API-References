---
title: "Calendar.GetStartDateFromFinishAndDuration"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Calendar method. Restituisce la data di inizio basata sulla data di fine e sulla durata specificate"
type: docs
weight: 200
url: /it/net/aspose.tasks/calendar/getstartdatefromfinishandduration/
---
## GetStartDateFromFinishAndDuration(DateTime, Duration) {#getstartdatefromfinishandduration}

Restituisce la data di inizio basata sulla data di fine e sulla durata specificate.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, Duration duration)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fine | DateTime | La data di fine specificata. |
| durata | Durata | La durata specificata. |

### Valore di ritorno

Data di inizio calcolata.

## Esempi

Mostra come ottenere una data di inizio a partire dalla data di fine e dalla durata.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// ottieni la data di inizio dalla data di fine e da una durata
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), project.GetDuration(16, TimeUnitType.Hour));

// 8 aprile 2020 09:00 verrà stampato
Console.WriteLine(startDate);
```

### Vedi anche

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetStartDateFromFinishAndDuration(DateTime, TimeSpan) {#getstartdatefromfinishandduration_1}

Restituisce la data di inizio basata sulla data di fine e sulla durata specificate.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, TimeSpan duration)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fine | DateTime | La data di fine specificata. |
| durata | TimeSpan | La durata specificata. |

### Valore di ritorno

Data di inizio calcolata.

## Esempi

Mostra come ottenere una data di inizio a partire dalla data di fine e dalla durata (come intervallo di tempo).

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// ottieni la data di inizio dalla data di fine e da una durata
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), TimeSpan.FromHours(16));

// 8 aprile 2020 09:00 verrà stampato
Console.WriteLine(startDate);
```

### Vedi anche

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


