---
title: "TaskCollection.Add"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode TaskCollection. Ajoute la tâche spécifiée à l'instance de la classe TaskCollection. Si ParentProject.CalculationMode est None, l'utilisateur doit appeler Project.Recalculate() après avoir utilisé cette méthode. Elle replanifiera toutes les dates de début/fin des tâches du projet, définira les dates anticipées/retardées et calculera les champs dépendants tels que les marges, le travail et les champs de coût, les identifiants et les niveaux de plan. Si ParentProject.CalculationMode est Manual, la méthode calculera uniquement l'identifiant de la tâche, le niveau de plan et les numéros de plan automatiquement. Si ParentProject.CalculationMode est Automatic, la méthode replanifiera automatiquement toutes les tâches du projet (dates de début/fin, dates anticipées/retardées), calculera les marges, le travail et les champs de coût, et recalculera les identifiants et les niveaux de plan."
type: docs
weight: 50
url: /fr/net/aspose.tasks/taskcollection/add/
---
## Add(Task) {#add_4}

Ajoute la tâche spécifiée à l'instance de la classe [`TaskCollection`](../). Si ParentProject.CalculationMode est None, l'utilisateur doit appeler Project.Recalculate() après avoir utilisé cette méthode (cela replanifiera toutes les tâches du projet (dates de début/fin, dates anticipées/retardées) et calculera les champs dépendants tels que les marges, le travail et les champs de coût, les identifiants et les niveaux de plan). Si ParentProject.CalculationMode est Manual, la méthode calculera uniquement l'identifiant de la tâche, le niveau de plan et les numéros de plan automatiquement. Si ParentProject.CalculationMode est Automatic, la méthode replanifiera automatiquement toutes les tâches du projet (dates de début/fin, dates anticipées/retardées, calcul des marges, du travail et des champs de coût, recalcul des identifiants et des niveaux de plan).

```csharp
public void Add(Task item)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| élément | Tâche | la tâche spécifiée qui doit être ajoutée à cette collection de tâches. |

## Exemples

Montre comment déplacer une tâche sous un autre parent.

```csharp
var project = new Project(DataDir + "MoveTask.mpp") { CalculationMode = CalculationMode.Automatic };

// Obtenir les tâches par identifiants
var task = project.RootTask.Children.GetByUid(6);
var task2 = project.RootTask.Children.GetByUid(3);

// Ajout de la tâche 6 à un autre parent
task2.Children.Add(task);
```

### Voir aussi

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add() {#add}

Ajoute une nouvelle tâche à la collection de tâches du projet au même niveau de plan que la dernière tâche.

```csharp
public Task Add()
```

### Valeur de retour

renvoie la nouvelle instance de la classe [`Task`](../../task/).

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

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string) {#add_2}

Ajoute une nouvelle tâche à la collection des tâches enfants.

```csharp
public Task Add(string taskName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| taskName | Chaîne | le nom de tâche spécifié. |

### Valeur de retour

renvoie la nouvelle instance de la classe [`Task`](../../task/).

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

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, int) {#add_3}

Ajoute une nouvelle tâche récurrente à la collection des tâches enfants.

```csharp
public Task Add(string taskName, int beforeTaskId)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| taskName | Chaîne | le nom de tâche spécifié. |
| beforeTaskId | Int32 | L'identifiant spécifié d'une tâche avant laquelle une nouvelle tâche sera insérée. |

### Valeur de retour

renvoie une tâche qui a été insérée avant une tâche avec l'identifiant spécifié.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | ArgumentOutOfRangeException est levée si l'identifiant spécifié n'est pas un identifiant de tâche valide. |

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

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(RecurringTaskParameters) {#add_1}

Insère une nouvelle tâche avant une tâche avec l'ID spécifié et au même niveau de plan.

```csharp
public Task Add(RecurringTaskParameters parameters)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| parameters | RecurringTaskParameters | Les paramètres spécifiés pour la création d'une tâche récurrente. |

### Valeur de retour

renvoie la nouvelle instance de la classe [`Task`](../../task/).

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | Lancée si les paramètres spécifiés sont nuls. |
| ArgumentException | Lancée si les paramètres spécifiés sont invalides. |

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

* class [Task](../../task/)
* class [RecurringTaskParameters](../../recurringtaskparameters/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)


