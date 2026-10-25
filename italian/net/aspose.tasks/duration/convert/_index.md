---
title: "Duration.Convert"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Duration. Converte l'oggetto Duration in un'altra durata con le unità di tempo specificate"
type: docs
weight: 70
url: /it/net/aspose.tasks/duration/convert/
---
## Duration.Convert method

Converte l'oggetto Duration in un'altra durata con le unità di tempo specificate.

```csharp
public Duration Convert(TimeUnitType timeUnitType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| timeUnitType | TimeUnitType | il tipo di unità di tempo specificato. |

### Valore di ritorno

restituisce una nuova durata con il tipo di unità specificato.

## Esempi

Mostra come convertire una durata in diversi tipi di unità di tempo.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// Ottieni un'attività per calcolare la sua durata in diversi formati
var task = project.RootTask.Children.GetById(1);

// Ottieni la durata in minuti, giorni, ore, settimane e mesi
var mins = task.Get(Tsk.Duration).Convert(TimeUnitType.Minute).ToDouble();
Console.WriteLine("Duration in Mins: {0}", mins);
var days = task.Get(Tsk.Duration).Convert(TimeUnitType.Day).ToDouble();
Console.WriteLine("Duration in Days: {0}", days);
var hours = task.Get(Tsk.Duration).Convert(TimeUnitType.Hour).ToDouble();
Console.WriteLine("Duration in Hours: {0}", hours);
var weeks = task.Get(Tsk.Duration).Convert(TimeUnitType.Week).ToDouble();
Console.WriteLine("Duration in Weeks: {0}", weeks);
var months = task.Get(Tsk.Duration).Convert(TimeUnitType.Month).ToDouble();
Console.WriteLine("Duration in Months: {0}", months);
```

### Vedi anche

* enum [TimeUnitType](../../timeunittype/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


