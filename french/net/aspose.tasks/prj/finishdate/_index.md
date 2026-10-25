---
title: "Prj.FinishDate"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. La date de fin d'un projet"
type: docs
weight: 330
url: /fr/net/aspose.tasks/prj/finishdate/
---
## Prj.FinishDate field

La date de fin d'un projet.

```csharp
public static readonly Key<DateTime, PrjKey> FinishDate;
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
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


