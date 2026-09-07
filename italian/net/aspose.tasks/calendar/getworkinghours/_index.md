---
title: "Calendar.GetWorkingHours"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Calendar. Restituisce WorkUnit, Inizio, Fine e Durata delle ore lavorative per l'intervallo di data e ora specificato"
type: docs
weight: 220
url: /it/net/aspose.tasks/calendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

Restituisce WorkUnit - Inizio, Fine e Durata delle ore lavorative per l'intervallo di data/ora specificato.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | DateTime | Data di inizio dell'intervallo. |
| fine | DateTime | Data di fine dell'intervallo. |

### Valore di ritorno

Istanza della classe [`WorkUnit`](../../workunit/) contenente Start, Finish e Duration delle ore lavorative.

## Esempi

Mostra come ottenere le ore lavorative per date specifiche.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// ottieni le ore lavorative per una data specifica
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

// Verranno stampate 16 ore
Console.WriteLine(workUnit.WorkingHours);
```

### Vedi anche

* class [WorkUnit](../../workunit/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

Restituisce la quantità di ore lavorative nella data specificata.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dt | DateTime | La data per cui ottenere le ore lavorative. |

### Valore di ritorno

Ore lavorative nella data specificata.

## Esempi

Mostra come ottenere le ore lavorative per una data specifica.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// ottieni le ore lavorative per una data specifica
var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 10));

// Verranno stampate 8 ore
Console.WriteLine(workingHours.Hours);
```

### Vedi anche

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


