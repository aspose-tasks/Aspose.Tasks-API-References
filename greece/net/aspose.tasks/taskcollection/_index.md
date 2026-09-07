---
title: "Κλάση TaskCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.TaskCollection. Αντιπροσωπεύει μια συλλογή αντικειμένων Task"
type: docs
weight: 2390
url: /el/net/aspose.tasks/taskcollection/
---
## TaskCollection class

Αναπαριστά μια συλλογή από αντικείμενα [`Task`](../task/).

```csharp
public class TaskCollection : IList<Task>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/taskcollection/count/) { get; } | Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται στη TaskCollection. |
| [IsReadOnly](../../aspose.tasks/taskcollection/isreadonly/) { get; } | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση. |
| [Item](../../aspose.tasks/taskcollection/item/) { get; set; } | Επιστρέφει το στοιχείο στο καθορισμένο δείκτη. |
| [ParentProject](../../aspose.tasks/taskcollection/parentproject/) { get; } | Λαμβάνει το γονικό έργο του αντικειμένου TaskCollection. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/taskcollection/add/#add)() | Προσθέτει νέα εργασία στη συλλογή εργασιών του έργου στο ίδιο επίπεδο διάρθρωσης με την τελευταία εργασία. |
| [Add](../../aspose.tasks/taskcollection/add/#add_1)(RecurringTaskParameters) | Εισάγει μια νέα εργασία πριν από μια εργασία με το καθορισμένο id και στο ίδιο επίπεδο διάρθρωσης. |
| [Add](../../aspose.tasks/taskcollection/add/#add_2)(string) | Προσθέτει μια νέα εργασία στη συλλογή υποεργασιών. |
| [Add](../../aspose.tasks/taskcollection/add/#add_4)(Task) | Προσθέστε την καθορισμένη εργασία στην παρουσία της κλάσης `TaskCollection`. Εάν το ParentProject.CalculationMode είναι None, ο χρήστης πρέπει να καλέσει Project.Recalculate() μετά τη χρήση αυτής της μεθόδου (Θα προγραμματίσει εκ νέου όλες τις εργασίες του έργου (ημερομηνίες έναρξης/λήξης, ορίζει πρώιμες/αργές ημερομηνίες) και θα υπολογίσει τα εξαρτημένα πεδία όπως τα περιθώρια, τα πεδία εργασίας και κόστους, τα ids και τα επίπεδα διάρθρωσης). Εάν το ParentProject.CalculationMode είναι Manual, η μέθοδος θα υπολογίσει μόνο το id της εργασίας, το επίπεδο διάρθρωσης και τους αριθμούς διάρθρωσης αυτόματα. Εάν το ParentProject.CalculationMode είναι Automatic, η μέθοδος προγραμματίζει εκ νέου όλες τις εργασίες του έργου αυτόματα (ημερομηνίες έναρξης/λήξης, ορίζει πρώιμες/αργές ημερομηνίες, υπολογίζει τα περιθώρια, τα πεδία εργασίας και κόστους, επαναϋπολογίζει τα ids και τα επίπεδα διάρθρωσης). |
| [Add](../../aspose.tasks/taskcollection/add/#add_3)(string, int) | Προσθέτει μια νέα επαναλαμβανόμενη εργασία στη συλλογή υποεργασιών. |
| [Contains](../../aspose.tasks/taskcollection/contains/)(Task) | Ελέγχει εάν η συλλογή περιέχει το καθορισμένο στοιχείο. |
| [GetById](../../aspose.tasks/taskcollection/getbyid/)(int) | Επιστρέφει μια εργασία με το καθορισμένο Id του οποίου ο πρόγονος είναι η γονική εργασία αυτής της συλλογής. |
| [GetByUid](../../aspose.tasks/taskcollection/getbyuid/)(int) | Επιστρέφει μια εργασία με το καθορισμένο Uid του οποίου ο πρόγονος είναι η γονική εργασία αυτής της συλλογής. |
| [GetEnumerator](../../aspose.tasks/taskcollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [Insert](../../aspose.tasks/taskcollection/insert/)(int, Task) | Αυτή είναι η υλοποίηση stub της μεθόδου Insert του IList, η οποία μόνο ρίχνει NotSupportedException |
| [Remove](../../aspose.tasks/taskcollection/remove/)(Task) | Αυτή είναι η υλοποίηση stub της μεθόδου Remove του ICollection, η οποία μόνο ρίχνει NotSupportedException |
| [ToList](../../aspose.tasks/taskcollection/tolist/)() | Μετατρέπει το αντικείμενο TaskCollection σε λίστα αντικειμένων [`Task`](../task/). |

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

* class [Task](../task/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


