---
title: "Classe TaskCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.TaskCollection. Représente une collection d'objets Task"
type: docs
weight: 2390
url: /fr/net/aspose.tasks/taskcollection/
---
## TaskCollection class

Représente une collection d'objets [`Task`](../task/).

```csharp
public class TaskCollection : IList<Task>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/taskcollection/count/) { get; } | Obtient le nombre d'objets contenus dans la TaskCollection. |
| [IsReadOnly](../../aspose.tasks/taskcollection/isreadonly/) { get; } | Obtient une valeur indiquant si cette collection est en lecture seule. |
| [Item](../../aspose.tasks/taskcollection/item/) { get; set; } | Renvoie l'élément à l'index spécifié. |
| [ParentProject](../../aspose.tasks/taskcollection/parentproject/) { get; } | Obtient le projet parent de l'objet TaskCollection. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks/taskcollection/add/#add)() | Ajoute une nouvelle tâche à la collection de tâches du projet au même niveau de plan que la dernière tâche. |
| [Add](../../aspose.tasks/taskcollection/add/#add_1)(RecurringTaskParameters) | Insère une nouvelle tâche avant une tâche avec l'ID spécifié et au même niveau de plan. |
| [Add](../../aspose.tasks/taskcollection/add/#add_2)(string) | Ajoute une nouvelle tâche à la collection des tâches enfants. |
| [Add](../../aspose.tasks/taskcollection/add/#add_4)(Task) | Ajoutez la tâche spécifiée à l'instance de la classe `TaskCollection`. Si ParentProject.CalculationMode est None, l'utilisateur doit appeler Project.Recalculate() après avoir utilisé cette méthode (cela replanifiera toutes les tâches du projet (dates de début/fin, définit les dates anticipées/tardives) et calculera les champs dépendants tels que les marges, le travail et les champs de coût, les identifiants et les niveaux de plan). Si ParentProject.CalculationMode est Manual, la méthode calculera uniquement l'identifiant de la tâche, le niveau de plan et les numéros de plan automatiquement. Si ParentProject.CalculationMode est Automatic, la méthode replanifie automatiquement toutes les tâches du projet (dates de début/fin, définit les dates anticipées/tardives, calcule les marges, le travail et les champs de coût, recalculera les identifiants et les niveaux de plan). |
| [Add](../../aspose.tasks/taskcollection/add/#add_3)(string, int) | Ajoute une nouvelle tâche récurrente à la collection des tâches enfants. |
| [Contains](../../aspose.tasks/taskcollection/contains/)(Task) | Vérifie si la collection contient l'élément spécifié. |
| [GetById](../../aspose.tasks/taskcollection/getbyid/)(int) | Renvoie une tâche avec l'Id spécifié dont l'ancêtre est la tâche parent de cette collection. |
| [GetByUid](../../aspose.tasks/taskcollection/getbyuid/)(int) | Renvoie une tâche avec l'Uid spécifié dont l'ancêtre est la tâche parent de cette collection. |
| [GetEnumerator](../../aspose.tasks/taskcollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [Insert](../../aspose.tasks/taskcollection/insert/)(int, Task) | Ceci est l'implémentation factice de la méthode Insert de IList, qui ne lance que NotSupportedException |
| [Remove](../../aspose.tasks/taskcollection/remove/)(Task) | Ceci est l'implémentation factice de la méthode Remove de ICollection, qui ne lance que NotSupportedException |
| [ToList](../../aspose.tasks/taskcollection/tolist/)() | Convertit l'objet TaskCollection en une liste d'objets [`Task`](../task/). |

## Exemples

Montre comment travailler avec les collections de tâches.

```csharp
var project = new Project();

// la collection de tâches n'est pas en lecture seule et peut être étendue
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// créer des tâches
var task1 = project.RootTask.Children.Add();
task1.Set(Tsk.Name, "Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task1.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task3.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task3.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2", 2);
task2.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// imprimer les tâches du projet
Console.WriteLine("Count of tasks: " + project.RootTask.Children.Count);
foreach (var child in project.RootTask.Children)
{
    Console.WriteLine("Parent Project: " + project.RootTask.ParentProject.Get(Prj.Name));
    Console.WriteLine("Task name: " + child.Get(Tsk.Name));
    Console.WriteLine("Task start: " + child.Get(Tsk.Start));
    Console.WriteLine("Task duration: " + child.Get(Tsk.Duration));
    Console.WriteLine("Task finish: " + child.Get(Tsk.Finish));
    Console.WriteLine();
}

// une tâche peut être récupérée de la collection par ID
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// ou par UID
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// on peut également ajouter une tâche récurrente
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2020, 4, 13, 8, 0, 0),
                                                                               Finish = new DateTime(2021, 4, 13, 17, 0, 0)
                                                                           }
                                                 }
                     };

// la première tâche d'une séquence est renvoyée
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// la collection peut être convertie en une liste simple
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### Voir aussi

* class [Task](../task/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


