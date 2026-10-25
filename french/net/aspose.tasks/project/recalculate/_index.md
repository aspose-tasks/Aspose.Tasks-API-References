---
title: "Project.Recalculate"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode du projet. Replanifie toutes les tâches du projet, les identifiants, les niveaux de contour, les dates de début/fin, définit les dates anticipées/retardées, calcule les marges, le travail et les champs de coût."
type: docs
weight: 1150
url: /fr/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

Replanifie les identifiants, les niveaux d’outline, les dates de début/fin de toutes les tâches du projet, définit les dates anticipées/retardées, calcule les marges, le travail et les champs de coût.

```csharp
public void Recalculate()
```

## Exemples

Montre comment replanifier le projet à partir de la date de début au lieu de la date de fin.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, new DateTime(2014, 1, 1));

// Désormais, toutes les dates des tâches (Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish) sont calculées. Pour obtenir le chemin critique, nous devons calculer les marges (peut être invoqué dans un thread séparé, mais uniquement après le calcul de toutes les dates anticipées/retardées).
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Voir aussi

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

Replanifie les identifiants, les niveaux d’outline, les dates de début/fin de toutes les tâches du projet, définit les dates anticipées/retardées, calcule les marges, le travail et les champs de coût avec une validation facultative.

```csharp
public void Recalculate(bool validate)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| validate | Boolean | Si vrai, la validation du recalcul sera effectuée. Quelles données sont validées : pour le moment, seule la validation de base des intervalles de dates des tâches et des liaisons de tâches est implémentée. Les intervalles de dates des tâches (par ex. ActualStart - ActualFinish, EarlyStart - EarlyFinish, etc.) ainsi que les dates des liaisons de tâches seront vérifiés selon le critère selon lequel la date de début doit être inférieure ou égale à la date de fin. Si l’une des conditions décrites ci‑dessus échoue, alors [`RecalculationValidationException`](../../recalculationvalidationexception/) sera levée. |

## Exemples

Montre comment recalculer le projet avec une validation postérieure.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("t1");
task.Set(Tsk.CommitmentStart, new DateTime(2017, 6, 19, 8, 0, 0));
task.Set(Tsk.CommitmentFinish, new DateTime(2017, 6, 18, 17, 0, 0));

try
{
    // recalculer le projet avec une validation postérieure
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Voir aussi

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


