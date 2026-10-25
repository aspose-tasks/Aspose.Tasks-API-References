---
title: "Prj.ScheduleFromStart"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine s'il faut calculer le planning du projet à partir de la date de début"
type: docs
weight: 630
url: /fr/net/aspose.tasks/prj/schedulefromstart/
---
## Prj.ScheduleFromStart field

Détermine si le calendrier du projet doit être calculé en avant à partir de la date de début.

```csharp
public static readonly Key<NullableBool, PrjKey> ScheduleFromStart;
```

## Exemples

Montre comment replanifier le projet à partir de la date de fin au lieu de la date de début.

```csharp
var project = new Project();
project.Set(Prj.ScheduleFromStart, false);
project.Set(Prj.FinishDate, new DateTime(2020, 1, 1));

// Désormais, toutes les dates des tâches (Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish) sont calculées. Pour obtenir le chemin critique, nous devons calculer les marges (peut être invoqué dans un thread séparé, mais uniquement après le calcul de toutes les dates anticipées/retardées).
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


