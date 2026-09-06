---
title: "Project.UpdateProjectWorkAsComplete"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Project. Met à jour tout le travail comme terminé jusqu'à une date spécifiée pour l'ensemble du projet"
type: docs
weight: 1270
url: /fr/net/aspose.tasks/project/updateprojectworkascomplete/
---
## UpdateProjectWorkAsComplete(DateTime, bool) {#updateprojectworkascomplete}

Marque tout le travail comme terminé jusqu’à une date spécifiée pour l’ensemble du projet.

```csharp
public void UpdateProjectWorkAsComplete(DateTime completeThrough, 
    bool setZeroOrHundredPercentCompleteOnly)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| completeThrough | DateTime | La date jusqu'à laquelle mettre à jour le travail comme terminé. |
| setZeroOrHundredPercentCompleteOnly | Boolean | Si défini sur true, ne met à jour que les tâches comme 100 % terminées dont la date de fin est antérieure à la date de fin spécifiée. Sinon, calcule une valeur de pourcentage d'achèvement basée sur les dates de début planifiées et la date de fin spécifiée. |

## Exemples

Montre comment mettre à jour le projet et replanifier le travail non terminé.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2014, 1, 27, 8, 0, 0));

// Ajouter de nouvelles tâches
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Duration, task2.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task4 = project.RootTask.Children.Add("Task 4");
task4.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task5 = project.RootTask.Children.Add("Task 5");
task5.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));

// Ajouter des liens entre les tâches
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);
var link23 = project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);

// Retard d'un jour
link23.LinkLag = 4800;
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart);

// Ajouter de nouvelles tâches
var task6 = project.RootTask.Children.Add("Task 6");
var task7 = project.RootTask.Children.Add("Task 7");
task7.Set(Tsk.Duration, task7.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task8 = project.RootTask.Children.Add("Task 8");
task8.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task9 = project.RootTask.Children.Add("Task 9");
task9.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task10 = project.RootTask.Children.Add("Task 10");

// Ajouter des liens entre les tâches
project.TaskLinks.Add(task6, task7, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task7, task8, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task8, task9, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task9, task10, TaskLinkType.FinishToStart);
task6.Set(Tsk.IsManual, true);
task7.Set(Tsk.IsManual, true);
task8.Set(Tsk.IsManual, true);
task9.Set(Tsk.IsManual, true);
task10.Set(Tsk.IsManual, true);

// Enregistrer le projet avant et après la mise à jour du travail comme terminé
project.Save(OutDir + "RescheduleUncompletedWork_not updated_out.xml", SaveFileFormat.Xml);

// Enregistrer le projet après avoir mis à jour le travail du projet comme terminé uniquement pour les tâches spécifiées
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false, new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_updated_out.xml", SaveFileFormat.Xml);

// Enregistrer le projet après avoir mis à jour tout le travail du projet comme terminé
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false);
project.Save(OutDir + "RescheduleUncompletedWork_updated_out.xml", SaveFileFormat.Xml);

// Enregistrer le projet après avoir replanifié le travail non terminé uniquement pour les tâches spécifiées
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 8, 8, 0, 0), new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_rescheduled_out.xml", SaveFileFormat.Xml);

// Enregistrer le projet après avoir replanifié le travail non terminé
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 7, 8, 0, 0));
project.Save(OutDir + "RescheduleUncompletedWork_rescheduled_out.xml", SaveFileFormat.Xml);
```

### Voir aussi

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## UpdateProjectWorkAsComplete(DateTime, bool, List&lt;Task&gt;) {#updateprojectworkascomplete_1}

Marque tout le travail comme terminé jusqu’à une date spécifiée pour la liste de tâches spécifiée.

```csharp
public void UpdateProjectWorkAsComplete(DateTime completeThrough, 
    bool setZeroOrHundredPercentCompleteOnly, List<Task> taskCollection)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| completeThrough | DateTime | La date jusqu'à laquelle mettre à jour le travail comme terminé. |
| setZeroOrHundredPercentCompleteOnly | Boolean | Si défini sur true, ne met à jour que les tâches comme 100 % terminées dont la date de fin est antérieure à la date de fin spécifiée. Sinon, calcule une valeur de pourcentage d'achèvement basée sur les dates de début planifiées et la date de fin spécifiée. |
| taskCollection | List`1 | List&lt;Task&gt; des tâches pour lesquelles mettre à jour le travail. |

## Exemples

Montre comment mettre à jour le projet et replanifier le travail non terminé.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2014, 1, 27, 8, 0, 0));

// Ajouter de nouvelles tâches
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Duration, task2.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task4 = project.RootTask.Children.Add("Task 4");
task4.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task5 = project.RootTask.Children.Add("Task 5");
task5.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));

// Ajouter des liens entre les tâches
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);
var link23 = project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);

// Retard d'un jour
link23.LinkLag = 4800;
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart);

// Ajouter de nouvelles tâches
var task6 = project.RootTask.Children.Add("Task 6");
var task7 = project.RootTask.Children.Add("Task 7");
task7.Set(Tsk.Duration, task7.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task8 = project.RootTask.Children.Add("Task 8");
task8.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task9 = project.RootTask.Children.Add("Task 9");
task9.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task10 = project.RootTask.Children.Add("Task 10");

// Ajouter des liens entre les tâches
project.TaskLinks.Add(task6, task7, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task7, task8, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task8, task9, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task9, task10, TaskLinkType.FinishToStart);
task6.Set(Tsk.IsManual, true);
task7.Set(Tsk.IsManual, true);
task8.Set(Tsk.IsManual, true);
task9.Set(Tsk.IsManual, true);
task10.Set(Tsk.IsManual, true);

// Enregistrer le projet avant et après la mise à jour du travail comme terminé
project.Save(OutDir + "RescheduleUncompletedWork_not updated_out.xml", SaveFileFormat.Xml);

// Enregistrer le projet après avoir mis à jour le travail du projet comme terminé uniquement pour les tâches spécifiées
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false, new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_updated_out.xml", SaveFileFormat.Xml);

// Enregistrer le projet après avoir mis à jour tout le travail du projet comme terminé
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false);
project.Save(OutDir + "RescheduleUncompletedWork_updated_out.xml", SaveFileFormat.Xml);

// Enregistrer le projet après avoir replanifié le travail non terminé uniquement pour les tâches spécifiées
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 8, 8, 0, 0), new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_rescheduled_out.xml", SaveFileFormat.Xml);

// Enregistrer le projet après avoir replanifié le travail non terminé
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 7, 8, 0, 0));
project.Save(OutDir + "RescheduleUncompletedWork_rescheduled_out.xml", SaveFileFormat.Xml);
```

### Voir aussi

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


