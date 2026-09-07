---
title: "Duration.Add"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Duration metodo. Aggiunge la durata specificata a questa durata"
type: docs
weight: 60
url: /it/net/aspose.tasks/duration/add/
---
## Add(Duration) {#add}

Aggiunge la durata specificata a questa durata.

```csharp
public Duration Add(Duration d)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| d | Duration | durata specificata [`Duration`](../) da aggiungere a questa istanza. |

### Valore di ritorno

Nuovo oggetto durata che rappresenta il valore di questa istanza più il valore di durata specificato.

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

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Add(double) {#add_1}

Aggiunge il valore double specificato a questa durata.

```csharp
public Duration Add(double val)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| val | Double | il valore Double specificato da aggiungere a questa istanza. |

### Valore di ritorno

Nuovo oggetto durata che rappresenta il valore di questa istanza più il valore di durata specificato.

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

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


