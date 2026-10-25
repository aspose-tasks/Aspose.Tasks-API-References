---
title: "Klasse TaskCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.TaskCollection klasse. Vertegenwoordigt een collectie van Task-objecten"
type: docs
weight: 2390
url: /nl/net/aspose.tasks/taskcollection/
---
## TaskCollection class

Vertegenwoordigt een collectie van [`Task`](../task/) objecten.

```csharp
public class TaskCollection : IList<Task>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/taskcollection/count/) { get; } | Haalt het aantal objecten op dat in de TaskCollection zit. |
| [IsReadOnly](../../aspose.tasks/taskcollection/isreadonly/) { get; } | Geeft een waarde terug die aangeeft of deze collectie alleen‑lezen is. |
| [Item](../../aspose.tasks/taskcollection/item/) { get; set; } | Retourneert het element op de opgegeven index. |
| [ParentProject](../../aspose.tasks/taskcollection/parentproject/) { get; } | Haalt het bovenliggende project op van het TaskCollection-object. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/taskcollection/add/#add)() | Voegt een nieuwe taak toe aan de projecttakenverzameling op hetzelfde outline-niveau als de laatste taak. |
| [Add](../../aspose.tasks/taskcollection/add/#add_1)(RecurringTaskParameters) | Voegt een nieuwe taak in vóór een taak met de opgegeven id en op hetzelfde outline-niveau. |
| [Add](../../aspose.tasks/taskcollection/add/#add_2)(string) | Voegt een nieuwe taak toe aan de verzameling van onderliggende taken. |
| [Add](../../aspose.tasks/taskcollection/add/#add_4)(Task) | Voeg de opgegeven taak toe aan de instantie van de `TaskCollection`-klasse. Als ParentProject.CalculationMode None is, moet de gebruiker Project.Recalculate() aanroepen na het gebruik van deze methode (dit zal alle projecttaken opnieuw plannen (start-/einddatums, stelt vroege/late datums in) en de afhankelijke velden berekenen, zoals slack, werk- en kostengegevens, id's en outline-niveaus). Als ParentProject.CalculationMode Manual is, berekent de methode alleen taak-id, outline-niveau en outline-nummers automatisch. Als ParentProject.CalculationMode Automatic is, plant de methode alle taken van het project automatisch opnieuw (start-/einddatums, stelt vroege/late datums in, berekent slack, werk- en kostengegevens, herberekent id's en outline-niveaus). |
| [Add](../../aspose.tasks/taskcollection/add/#add_3)(string, int) | Voegt een nieuwe terugkerende taak toe aan de verzameling van onderliggende taken. |
| [Contains](../../aspose.tasks/taskcollection/contains/)(Task) | Controleert of de collectie het opgegeven item bevat. |
| [GetById](../../aspose.tasks/taskcollection/getbyid/)(int) | Retourneert een taak met de opgegeven Id waarvan de voorouder de bovenliggende taak van deze collectie is. |
| [GetByUid](../../aspose.tasks/taskcollection/getbyuid/)(int) | Retourneert een taak met de opgegeven Uid waarvan de voorouder de bovenliggende taak van deze collectie is. |
| [GetEnumerator](../../aspose.tasks/taskcollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [Insert](../../aspose.tasks/taskcollection/insert/)(int, Task) | Dit is de stub-implementatie van de Insert-methode van IList, die alleen NotSupportedException gooit. |
| [Remove](../../aspose.tasks/taskcollection/remove/)(Task) | Dit is de stub-implementatie van de Remove-methode van ICollection, die alleen NotSupportedException gooit. |
| [ToList](../../aspose.tasks/taskcollection/tolist/)() | Converteert het TaskCollection-object naar een lijst van [`Task`](../task/) objecten. |

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

* class [Task](../task/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


