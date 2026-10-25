---
title: "ResourceAssignment.TimephasedDataFromTaskDuration"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ResourceAssignment. Génère une liste de données à phases temporelles basée sur la durée de la tâche et la date de début prévue."
type: docs
weight: 780
url: /fr/net/aspose.tasks/resourceassignment/timephaseddatafromtaskduration/
---
## ResourceAssignment.TimephasedDataFromTaskDuration method

Génère une liste de données phasées dans le temps basée sur la durée de la tâche et la date de début planifiée.

```csharp
public void TimephasedDataFromTaskDuration(Calendar calendar)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| calendrier | Calendar | Le calendrier à partir duquel générer les données à phases temporelles. |

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


