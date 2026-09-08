---
title: "TaskCollection.GetById"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskCollection-methode. Geeft een taak terug met de opgegeven Id waarvan de voorouder de bovenliggende taak van deze collectie is."
type: docs
weight: 70
url: /nl/net/aspose.tasks/taskcollection/getbyid/
---
## TaskCollection.GetById method

Retourneert een taak met de opgegeven Id waarvan de voorouder de bovenliggende taak van deze collectie is.

```csharp
public Task GetById(int id)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| id | Int32 | TaskEntity Id |

### Retourwaarde

retourneert de instantie van de [`Task`](../../task/) klasse met de opgegeven id waarvan de voorouder de bovenliggende taak van deze collectie is.

## Voorbeelden

Toont hoe te werken met taakcollecties.

```csharp
var project = new Project();

// de taakcollectie is niet alleen-lezen en kan worden uitgebreid
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// taken maken
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

// projecttaken afdrukken
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

// een taak kan uit de collectie worden gehaald op basis van ID
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// of op basis van UID
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// ook kan men een terugkerende taak toevoegen
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

// de eerste taak in een reeks wordt geretourneerd
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// de collectie kan worden geconverteerd naar een eenvoudige lijst
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### Zie ook

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)


