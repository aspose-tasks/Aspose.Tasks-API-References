---
title: "Duration.Subtract"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Duration. Soustrait la durée spécifiée de cette instance de durée."
type: docs
weight: 100
url: /fr/net/aspose.tasks/duration/subtract/
---
## Subtract(Duration) {#subtract}

Soustrait la durée spécifiée de cette instance de durée.

```csharp
public Duration Subtract(Duration d)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| d | Duration | l'instance [`Duration`](../) spécifiée à soustraire de cette instance. |

### Valeur de retour

Nouvel objet Duration qui représente la valeur de cette instance moins la valeur de durée spécifiée.

## Exemples

Montre comment modifier une durée de tâches.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// obtenir une tâche
var task1 = project.RootTask.Children.GetById(1);

// mettre à jour la durée de la tâche
var duration1 = task1.Get(Tsk.Duration);

// soustraire un jour à la tâche 1
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// définir une nouvelle durée pour la tâche
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// obtenir une autre tâche
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// modifier la durée en utilisant le type d'unité de temps réel
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// définir une nouvelle durée pour la tâche
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### Voir aussi

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Subtract(double) {#subtract_1}

Soustrait la valeur double spécifiée de cette instance de durée.

```csharp
public Duration Subtract(double val)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| val | Double | valeur Double spécifiée à soustraire de cette instance. |

### Valeur de retour

Nouvel objet Duration qui représente la valeur de cette instance moins la valeur de durée spécifiée.

## Exemples

Montre comment modifier une durée de tâches.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// obtenir une tâche
var task1 = project.RootTask.Children.GetById(1);

// mettre à jour la durée de la tâche
var duration1 = task1.Get(Tsk.Duration);

// soustraire un jour à la tâche 1
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// définir une nouvelle durée pour la tâche
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// obtenir une autre tâche
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// modifier la durée en utilisant le type d'unité de temps réel
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// définir une nouvelle durée pour la tâche
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### Voir aussi

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


