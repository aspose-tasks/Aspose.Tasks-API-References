---
title: "Project.DefaultWeekWorkingDays"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Project. Obtient l'instance de la classe WeekDayCollection qui représente une collection des jours ouvrables hebdomadaires par défaut du projet et des horaires de travail"
type: docs
weight: 370
url: /fr/net/aspose.tasks/project/defaultweekworkingdays/
---
## Project.DefaultWeekWorkingDays property

Obtient l'instance de la classe [`WeekDayCollection`](../../weekdaycollection/) qui représente une collection des jours ouvrables hebdomadaires par défaut du projet et des horaires de travail.

```csharp
public WeekDayCollection DefaultWeekWorkingDays { get; }
```

### Valeur de retour

L'instance de la classe [`WeekDayCollection`](../../weekdaycollection/) qui contient une liste d'objets [`WeekDay`](../../weekday/).

## Remarques

Les données ne se trouvent que dans les fichiers mpp (pas dans xml).

## Exemples

Montre comment obtenir le jour ouvrable hebdomadaire par défaut.

```csharp
var project = new Project(DataDir + "Project2003.mpp");
foreach (var weekDay in project.DefaultWeekWorkingDays)
{
    Console.WriteLine("From: " + weekDay.FromDate);
    Console.WriteLine("From: " + weekDay.ToDate);
    Console.WriteLine("Day type: " + weekDay.DayType);
    Console.WriteLine("Is day working: " + weekDay.DayWorking);
}
```

### Voir aussi

* class [WeekDayCollection](../../weekdaycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


