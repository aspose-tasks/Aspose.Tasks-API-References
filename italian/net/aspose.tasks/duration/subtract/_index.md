---
title: "Duration.Subtract"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Duration. Sottrae la durata specificata da questa istanza di Duration"
type: docs
weight: 100
url: /it/net/aspose.tasks/duration/subtract/
---
## Subtract(Duration) {#subtract}

Sottrae la durata specificata da questa istanza di durata.

```csharp
public Duration Subtract(Duration d)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| d | Duration | l'istanza [`Duration`](../) specificata da sottrarre da questa istanza. |

### Valore di ritorno

Nuovo oggetto Duration che rappresenta il valore di questa istanza meno il valore della durata specificata.

## Esempi

Mostra come modificare la durata delle attività.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// ottieni un'attività
var task1 = project.RootTask.Children.GetById(1);

// aggiorna la durata dell'attività
var duration1 = task1.Get(Tsk.Duration);

// sottrai un giorno all'attività 1
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// imposta una nuova durata per l'attività
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// ottieni un'altra attività
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// cambia la durata usando il tipo di unità di tempo attuale
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// imposta una nuova durata per l'attività
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### Vedi anche

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Subtract(double) {#subtract_1}

Sottrae il valore double specificato da questa istanza di durata.

```csharp
public Duration Subtract(double val)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| val | Double | valore Double specificato da sottrarre da questa istanza. |

### Valore di ritorno

Nuovo oggetto Duration che rappresenta il valore di questa istanza meno il valore della durata specificata.

## Esempi

Mostra come modificare la durata delle attività.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// ottieni un'attività
var task1 = project.RootTask.Children.GetById(1);

// aggiorna la durata dell'attività
var duration1 = task1.Get(Tsk.Duration);

// sottrai un giorno all'attività 1
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// imposta una nuova durata per l'attività
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// ottieni un'altra attività
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// cambia la durata usando il tipo di unità di tempo attuale
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// imposta una nuova durata per l'attività
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### Vedi anche

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


