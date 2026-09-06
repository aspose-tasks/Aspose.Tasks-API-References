---
title: "Project.CalculationMode"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Project. Obtient ou définit le mode de calcul d'un projet. Peut être l'une des valeurs de l'énumération CalculationMode"
type: docs
weight: 110
url: /fr/net/aspose.tasks/project/calculationmode/
---
## Project.CalculationMode property

Obtient ou définit le mode de calcul d'un projet. Peut être l'une des valeurs de l'énumération `CalculationMode`.

```csharp
public CalculationMode CalculationMode { get; set; }
```

## Exemples

Montre comment utiliser le mode de calcul du projet.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Manual
};

// Définissez la date de début du projet et ajoutez de nouvelles tâches
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// Les propriétés nécessaires sont définies en mode manuel
Console.WriteLine("Task1.Id Equals 1 : {0} ", task1.Get(Tsk.Id).Equals(1));
Console.WriteLine("Task1 OutlineLevel Equals 1 : {0} ", task1.Get(Tsk.OutlineLevel).Equals(1));
Console.WriteLine("Task1 Start Equals 15/04/2015 08:00 AM : {0} ", task1.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task1 Finish Equals 15/04/2015 05:00 PM : {0} ", task1.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task1 Duration Equals 1 day : {0} ", task1.Get(Tsk.Duration).ToString().Equals("1 day"));
Console.WriteLine("Task2 Start Equals 15/04/2015 08:00 AM : {0} ", task2.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task2 Finish Equals 15/04/2015 05:00 PM : {0} ", task2.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task2 Duration Equals 1 day : {0} ", task2.Get(Tsk.Duration).ToString().Equals("1 day"));

// Lorsque nous lions deux tâches ensemble, leurs dates ne sont pas recalculées en mode manuel
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// Le début de la tâche 2 n'a pas été modifié
Console.WriteLine("Task1 Start Equals Task2 Start : {0} ", task1.Get(Tsk.Start).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).Equals(task2.Get(Tsk.Finish)));
```

### Voir aussi

* enum [CalculationMode](../../calculationmode/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


