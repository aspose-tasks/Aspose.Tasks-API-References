---
title: "Énumération WorkContourType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.WorkContourType. Spécifie le contour d'un travail"
type: docs
weight: 3610
url: /fr/net/aspose.tasks/workcontourtype/
---
## WorkContourType enumeration

Spécifie le contour d'un travail.

```csharp
public enum WorkContourType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Undefined | `-1` | La valeur n'était pas définie dans le fichier de projet original. |
| Flat | `0` | Contour de travail plat. |
| BackLoaded | `1` | Contour de travail chargé à l'arrière. |
| FrontLoaded | `2` | Contour de travail chargé à l'avant. |
| DoublePeak | `3` | Contour de travail à double pic. |
| EarlyPeak | `4` | Contour de travail à pic précoce. |
| LatePeak | `5` | Contour de travail à pic tardif. |
| Bell | `6` | Contour de travail en cloche. |
| Turtle | `7` | Contour de travail en tortue. |
| Contoured | `8` | Contour de travail personnalisé. |

## Remarques

Lors de l'exportation vers XML, les valeurs Undefined seront éliminées du XML résultant.

## Exemples

Montre comment définir différents contours de données chronophases pour les affectations de ressources.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 1, 3, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 1, 7, 17, 0, 0));

// ajouter une tâche
var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task.Set(Tsk.Finish, new DateTime(2000, 1, 3, 17, 0, 0));

var resource = project.Resources.Add("Resource");

// ajouter une affectation de ressource
var resourceAssignment = project.ResourceAssignments.Add(task, resource);
resourceAssignment.Set(Asn.Start, new DateTime(2000, 1, 3, 8, 0, 0));
resourceAssignment.Set(Asn.Work, project.GetWork(8));
resourceAssignment.Set(Asn.Finish, new DateTime(2000, 1, 3, 17, 0, 0));

// Le contour plat est le contour par défaut
Console.WriteLine("Flat contour");

var collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Modifier le contour
Console.WriteLine("Turtle contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.Turtle);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Modifier le contour
Console.WriteLine("BackLoaded contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.BackLoaded);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Modifier le contour
Console.WriteLine("FrontLoaded contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.FrontLoaded);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Modifier le contour
Console.WriteLine("Bell contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.Bell);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Modifier le contour
Console.WriteLine("EarlyPeak contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.EarlyPeak);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Modifier le contour
Console.WriteLine("LatePeak contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.LatePeak);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// Modifier le contour
Console.WriteLine("DoublePeak contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.DoublePeak);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


