---
title: "Calendar.GetTaskFinishDateFromDuration"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Calendar. Calcule la date et l'heure de fin de la tâche à partir de ses parties de date de début et de la durée de travail"
type: docs
weight: 210
url: /fr/net/aspose.tasks/calendar/gettaskfinishdatefromduration/
---
## Calendar.GetTaskFinishDateFromDuration method

Calcule la date et l'heure de fin de la tâche à partir de sa date de début, de ses parties séparées et de la durée du travail.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tâche | Tâche | La tâche pour laquelle calculer la date de fin. |
| duration | TimeSpan | La durée à calculer. |

### Valeur de retour

Date de fin de la tâche pour la date de début et la durée données.

## Remarques

Renvoie DateTime.MinValue si la tâche est un résumé, nulle ou si sa date de début n'est pas définie.

## Exemples

Montre comment calculer la date de fin d'une tâche à l'aide d'une durée personnalisée.

```csharp
var project = new Project(DataDir + "SplitTaskFinishDate.mpp");

// Trouver une tâche fractionnée
var task = project.RootTask.Children.GetByUid(4);

// Trouver le calendrier du projet
var calendar = project.Get(Prj.Calendar);

// Calculer la date de fin d'une tâche avec différentes durées
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 8 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(8, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 16 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(16, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 24 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(24, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 28 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(28, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 32 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(32, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 46 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(46, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 61 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(61, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 75 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(75, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 80 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(80, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 120 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(120, 0, 0)));
Console.WriteLine(
    "Start Date: " + task.Get(Tsk.Start).ToShortDateString() + "\n+ Duration 150 hours\nFinish Date: "
    + calendar.GetTaskFinishDateFromDuration(task, new TimeSpan(150, 0, 0)));
```

### Voir aussi

* class [Task](../../task/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


