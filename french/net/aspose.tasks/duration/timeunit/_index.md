---
title: "Duration.TimeUnit"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Duration. Obtient le type d'unité de temps pour cet objet. Le type d'unité de temps de cette instance Duration."
type: docs
weight: 50
url: /fr/net/aspose.tasks/duration/timeunit/
---
## Duration.TimeUnit property

Obtient le type d'unité de temps pour cet objet. Le type d'unité de temps de cette instance Duration.

```csharp
public TimeUnitType TimeUnit { get; }
```

## Exemples

Montre comment mettre à jour une durée de tâches.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// obtenir une tâche
var task1 = project.RootTask.Children.GetById(1);

// mettre à jour la durée de la tâche
var duration1 = task1.Get(Tsk.Duration);

// ajouter un jour à la tâche 1
duration1 = duration1.Add(project.GetDuration(1, TimeUnitType.Day));

// définir une nouvelle durée pour la tâche
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// obtenir une autre tâche
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// modifier la durée en utilisant le type d'unité de temps réel
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Add(1d /* the time unit type of duration2 will be used */);

// définir une nouvelle durée pour la tâche
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task1.Get(Tsk.Duration));
```

### Voir aussi

* enum [TimeUnitType](../../timeunittype/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


