---
title: "Duration.Convert"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Duration. Convertit l'objet Duration en une autre durée avec les unités de temps spécifiées"
type: docs
weight: 70
url: /fr/net/aspose.tasks/duration/convert/
---
## Duration.Convert method

Convertit l'objet Duration en une autre durée avec les unités de temps spécifiées.

```csharp
public Duration Convert(TimeUnitType timeUnitType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| timeUnitType | TimeUnitType | le type d'unité de temps spécifié. |

### Valeur de retour

renvoie une nouvelle durée avec le type d'unité spécifié.

## Exemples

Montre comment convertir une durée en différents types d'unités de temps.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// Obtenez une tâche pour calculer sa durée dans différents formats
var task = project.RootTask.Children.GetById(1);

// Obtenez la durée en Minutes, Jours, Heures, Semaines et Mois
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

### Voir aussi

* enum [TimeUnitType](../../timeunittype/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


