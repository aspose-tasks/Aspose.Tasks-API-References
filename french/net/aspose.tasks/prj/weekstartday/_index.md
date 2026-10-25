---
title: "Prj.WeekStartDay"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Premier jour de la semaine"
type: docs
weight: 780
url: /fr/net/aspose.tasks/prj/weekstartday/
---
## Prj.WeekStartDay field

Premier jour de la semaine.

```csharp
public static readonly Key<DayType, PrjKey> WeekStartDay;
```

## Exemples

Montre comment lire/écrire les propriétés des jours de semaine du projet.

```csharp
var project = new Project(DataDir + "WriteWeekdayProperties.mpp");

// Définir les propriétés des jours de semaine
project.Set(Prj.WeekStartDay, DayType.Monday);
project.Set(Prj.DaysPerMonth, 24);
project.Set(Prj.MinutesPerDay, 540);
project.Set(Prj.MinutesPerWeek, 3240);

// Afficher les propriétés des jours de semaine
Console.WriteLine("Week Start Date: " + project.Get(Prj.WeekStartDay));
Console.WriteLine("Days Per Month: " + project.Get(Prj.DaysPerMonth));
Console.WriteLine("Minutes Per Day: " + project.Get(Prj.MinutesPerDay));
Console.WriteLine("Minutes Per Week: " + project.Get(Prj.MinutesPerWeek));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [DayType](../../daytype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


