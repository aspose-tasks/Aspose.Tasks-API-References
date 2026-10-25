---
title: "TaskCollection.GetByUid"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος TaskCollection. Επιστρέφει μια εργασία με το καθορισμένο Uid του οποίου ο πρόγονος είναι η γονική εργασία αυτής της συλλογής"
type: docs
weight: 80
url: /el/net/aspose.tasks/taskcollection/getbyuid/
---
## TaskCollection.GetByUid method

Επιστρέφει μια εργασία με το καθορισμένο Uid του οποίου ο πρόγονος είναι η γονική εργασία αυτής της συλλογής.

```csharp
public Task GetByUid(int uid)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| uid | Int32 | TaskEntity Uid. |

### Τιμή Επιστροφής

επιστρέφει το παράδειγμα της κλάσης [`Task`](../../task/) με το καθορισμένο uid του οποίου ο πρόγονος είναι η γονική εργασία αυτής της συλλογής.

## Παραδείγματα

Δείχνει πώς να εργαστείτε με συλλογές εργασιών.

```csharp
var project = new Project();

// η συλλογή εργασιών δεν είναι μόνο για ανάγνωση και μπορεί να επεκταθεί
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// δημιουργία εργασιών
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

// εκτύπωση εργασιών έργου
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

// μια εργασία μπορεί να ληφθεί από τη συλλογή με ID
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// ή με UID
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// επίσης μπορεί κανείς να προσθέσει μια επαναλαμβανόμενη εργασία
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

// επιστρέφεται η πρώτη εργασία σε μια ακολουθία
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// η συλλογή μπορεί να μετατραπεί σε απλή λίστα
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### Δείτε επίσης

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)


