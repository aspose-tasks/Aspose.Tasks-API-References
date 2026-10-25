---
title: "ResourceAssignment.SplitTask"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ResourceAssignment. Divise la tâche en deux parties"
type: docs
weight: 770
url: /fr/net/aspose.tasks/resourceassignment/splittask/
---
## ResourceAssignment.SplitTask method

Divise la tâche en deux parties.

```csharp
public void SplitTask(DateTime start, DateTime finish, Calendar calendar)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| début | DateTime | Le début de l'interruption de travail sur lequel se baser pour la division. |
| fin | DateTime | La fin de l'interruption de travail sur laquelle se baser pour la division. |
| calendrier | Calendar | Le calendrier sur lequel se baser pour la division. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | Lance une exception lorsque la date de début est antérieure à la date de début de l'affectation. |
| ArgumentOutOfRangeException | Lance une exception lorsque la date de fin est postérieure à la date de fin de l'affectation. |

## Exemples

Montre comment ajouter une division à une tâche.

```csharp
var project = new Project();

// Obtenir un calendrier standard
var calendar = project.Get(Prj.Calendar);

// Définir les paramètres de calendrier du projet
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 4, 21, 17, 0, 0));

// Ajouter une nouvelle tâche à la tâche racine
var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Duration, project.GetDuration(3));

// Créer une nouvelle affectation de ressource et générer des données à phases temporelles
var assignment = project.ResourceAssignments.Add(task, null);
assignment.TimephasedDataFromTaskDuration(calendar);

// Diviser la tâche en 3 parties.
// Fournir les arguments date de début et date de fin à la méthode SplitTask qui seront utilisés pour la division
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 16, 17, 0, 0), calendar);
assignment.SplitTask(new DateTime(2000, 3, 18, 8, 0, 0), new DateTime(2000, 3, 18, 17, 0, 0), calendar);
assignment.Set(Asn.WorkContour, WorkContourType.Contoured);

project.Save(OutDir + "CreateSplitTasks_out.xml", SaveFileFormat.Xml);
```

### Voir aussi

* class [Calendar](../../calendar/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


