---
title: "Struct Duration"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Struct Aspose.Tasks.Duration. Rappresenta la durata in un progetto."
type: docs
weight: 470
url: /it/net/aspose.tasks/duration/
---
## Duration structure

Rappresenta la durata in un progetto.

```csharp
public struct Duration : IEquatable<Duration>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [IsElapsed](../../aspose.tasks/duration/iselapsed/) { get; } | Ottiene un valore che indica se l'unità di tempo è trascorsa. Il flag che determina se questa istanza di Duration è trascorsa. |
| [IsEstimated](../../aspose.tasks/duration/isestimated/) { get; } | Ottiene un valore che indica se l'unità di tempo è stimata. Il flag che determina se questa istanza di Duration è stimata. |
| [TimeSpan](../../aspose.tasks/duration/timespan/) { get; } | Ottiene l'istanza [`TimeSpan`](./timespan/) di questo oggetto Duration. L'istanza TimeSpan di questo oggetto Duration. |
| [TimeUnit](../../aspose.tasks/duration/timeunit/) { get; } | Ottiene il tipo di unità di tempo per questo oggetto. Il tipo di unità di tempo di questa istanza Duration. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [Parse](../../aspose.tasks/duration/parse/)(Project, string) | Converte la stringa specificata nell'istanza della struct `Duration`. |
| [Add](../../aspose.tasks/duration/add/#add_1)(double) | Aggiunge il valore double specificato a questa durata. |
| [Add](../../aspose.tasks/duration/add/#add)(Duration) | Aggiunge la durata specificata a questa durata. |
| [Convert](../../aspose.tasks/duration/convert/)(TimeUnitType) | Converte l'oggetto Duration in un'altra durata con le unità di tempo specificate. |
| [Equals](../../aspose.tasks/duration/equals/#equals)(Duration) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| override [Equals](../../aspose.tasks/duration/equals/#equals_1)(object) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| override [GetHashCode](../../aspose.tasks/duration/gethashcode/)() | Restituisce un valore di hash code per questo oggetto. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract_1)(double) | Sottrae il valore double specificato da questa istanza di durata. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract)(Duration) | Sottrae la durata specificata da questa istanza di durata. |
| [ToDouble](../../aspose.tasks/duration/todouble/)() | Converte l'oggetto Duration in un valore Double. |
| override [ToString](../../aspose.tasks/duration/tostring/)() | Restituisce una rappresentazione stringa di questa istanza. |
| static [ParseTimeSpan](../../aspose.tasks/duration/parsetimespan/)(string) | Analizza la stringa di durata nel formato "PT--H--M--S--". |
| [operator ==](../../aspose.tasks/duration/op_equality/) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [operator !=](../../aspose.tasks/duration/op_inequality/) | Restituisce un valore che indica se questa istanza non è uguale a un oggetto specificato. |

## Esempi

Mostra come aggiornare una durata delle attività.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// ottieni un'attività
var task1 = project.RootTask.Children.GetById(1);

// aggiorna la durata dell'attività
var duration1 = task1.Get(Tsk.Duration);

// aggiungi un giorno all'attività 1
duration1 = duration1.Add(project.GetDuration(1, TimeUnitType.Day));

// imposta una nuova durata per l'attività
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// ottieni un'altra attività
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// cambia la durata usando il tipo di unità di tempo attuale
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Add(1d /* the time unit type of duration2 will be used */);

// imposta una nuova durata per l'attività
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task1.Get(Tsk.Duration));
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


