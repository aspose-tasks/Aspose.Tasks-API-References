---
title: "Calendar.GetFinishDateByStartAndWork"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Calendar. Calcola la data in cui il tempo di lavoro specificato sarà trascorso secondo il calendario"
type: docs
weight: 160
url: /it/net/aspose.tasks/calendar/getfinishdatebystartandwork/
---
## GetFinishDateByStartAndWork(DateTime, Duration) {#getfinishdatebystartandwork}

Calcola la data in cui il tempo di lavoro specificato sarà trascorso secondo il calendario.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, Duration work)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | DateTime | Data di inizio. |
| lavoro | Durata | Durata del lavoro. |

### Valore di ritorno

Data di fine.

## Esempi

Mostra come calcolare una data di fine a partire da data di inizio e lavoro usando un'istanza di Calendar.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// calcola la data di fine usando un calendario standard
var finish = calendar.GetFinishDateByStartAndWork(start, work);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### Vedi anche

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetFinishDateByStartAndWork(DateTime, TimeSpan) {#getfinishdatebystartandwork_1}

Calcola la data in cui il tempo di lavoro specificato sarà trascorso secondo il calendario.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, TimeSpan work)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | DateTime | Data di inizio. |
| lavoro | TimeSpan | Durata del lavoro. |

### Valore di ritorno

Data di fine.

## Esempi

Mostra come calcolare una data di fine a partire da data di inizio e lavoro (come intervallo di tempo) usando un'istanza di Calendar.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// calcola la data di fine usando un calendario standard
var finish = calendar.GetFinishDateByStartAndWork(start, work.TimeSpan);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### Vedi anche

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


