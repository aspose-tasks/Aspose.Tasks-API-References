---
title: "Structure Duration"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Structure Aspose.Tasks.Duration. Représente la durée dans un projet"
type: docs
weight: 470
url: /fr/net/aspose.tasks/duration/
---
## Duration structure

Représente la durée dans un projet.

```csharp
public struct Duration : IEquatable<Duration>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [IsElapsed](../../aspose.tasks/duration/iselapsed/) { get; } | Obtient une valeur indiquant si l’unité de temps est écoulée. Le drapeau qui détermine si cette instance Duration est écoulée. |
| [IsEstimated](../../aspose.tasks/duration/isestimated/) { get; } | Obtient une valeur indiquant si l’unité de temps est estimée. Le drapeau qui détermine si cette instance Duration est estimée. |
| [TimeSpan](../../aspose.tasks/duration/timespan/) { get; } | Obtient l'instance [`TimeSpan`](./timespan/) de cet objet Duration. L'instance TimeSpan de cet objet Duration. |
| [TimeUnit](../../aspose.tasks/duration/timeunit/) { get; } | Obtient le type d'unité de temps pour cet objet. Le type d'unité de temps de cette instance Duration. |

## Méthodes

| Nom | Description |
| --- | --- |
| static [Parse](../../aspose.tasks/duration/parse/)(Project, string) | Convertit la chaîne spécifiée en instance de la structure `Duration`. |
| [Add](../../aspose.tasks/duration/add/#add_1)(double) | Ajoute la valeur double spécifiée à cette durée. |
| [Add](../../aspose.tasks/duration/add/#add)(Duration) | Ajoute la durée spécifiée à cette durée. |
| [Convert](../../aspose.tasks/duration/convert/)(TimeUnitType) | Convertit l'objet Duration en une autre durée avec les unités de temps spécifiées. |
| [Equals](../../aspose.tasks/duration/equals/#equals)(Duration) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| override [Equals](../../aspose.tasks/duration/equals/#equals_1)(object) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| override [GetHashCode](../../aspose.tasks/duration/gethashcode/)() | Renvoie une valeur de code de hachage pour cet objet. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract_1)(double) | Soustrait la valeur double spécifiée de cette instance de durée. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract)(Duration) | Soustrait la durée spécifiée de cette instance de durée. |
| [ToDouble](../../aspose.tasks/duration/todouble/)() | Convertit l'objet Duration en valeur Double. |
| override [ToString](../../aspose.tasks/duration/tostring/)() | Renvoie une représentation sous forme de chaîne de cette instance. |
| static [ParseTimeSpan](../../aspose.tasks/duration/parsetimespan/)(string) | Analyse la chaîne de durée au format "PT--H--M--S--". |
| [operator ==](../../aspose.tasks/duration/op_equality/) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [operator !=](../../aspose.tasks/duration/op_inequality/) | Renvoie une valeur indiquant si cette instance n'est pas égale à un objet spécifié. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


