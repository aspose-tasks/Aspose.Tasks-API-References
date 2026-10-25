---
title: "TaskCollection.Add"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "TaskCollection μέθοδος. Προσθέτει την καθορισμένη εργασία στην παρουσία της κλάσης TaskCollection. Εάν το ParentProject.CalculationMode είναι None, ο χρήστης πρέπει να καλέσει Project.Recalculate μετά τη χρήση αυτής της μεθόδου. Θα επαναπρογραμματίσει όλες τις ημερομηνίες έναρξης/λήξης των εργασιών του έργου, θα ορίσει πρώιμες/αργότερες ημερομηνίες και θα υπολογίσει τα εξαρτημένα πεδία όπως οι καθυστερήσεις, η εργασία και τα πεδία κόστους, τα IDs και τα επίπεδα περιγράμματος. Εάν το ParentProject.CalculationMode είναι Manual, η μέθοδος θα υπολογίσει μόνο το ID της εργασίας, το επίπεδο περιγράμματος και τους αριθμούς περιγράμματος αυτόματα. Εάν το ParentProject.CalculationMode είναι Automatic, η μέθοδος επαναπρογραμματίζει αυτόματα όλες τις εργασίες του έργου (ημερομηνίες έναρξης/λήξης, ορίζει πρώιμες/αργότερες ημερομηνίες, υπολογίζει τις καθυστερήσεις, την εργασία και τα πεδία κόστους, επαναϋπολογίζει τα IDs και τα επίπεδα περιγράμματος)."
type: docs
weight: 50
url: /el/net/aspose.tasks/taskcollection/add/
---
## Add(Task) {#add_4}

Προσθέτει την καθορισμένη εργασία στην παρουσία της κλάσης [`TaskCollection`](../). Εάν το ParentProject.CalculationMode είναι None, ο χρήστης πρέπει να καλέσει Project.Recalculate() μετά τη χρήση αυτής της μεθόδου (Θα επαναπρογραμματίσει όλες τις εργασίες του έργου (ημερομηνίες έναρξης/λήξης, ορίζει πρώιμες/αργότερες ημερομηνίες) και θα υπολογίσει τα εξαρτημένα πεδία όπως οι καθυστερήσεις, η εργασία και τα πεδία κόστους, τα IDs και τα επίπεδα περιγράμματος). Εάν το ParentProject.CalculationMode είναι Manual, η μέθοδος θα υπολογίσει μόνο το ID της εργασίας, το επίπεδο περιγράμματος και τους αριθμούς περιγράμματος αυτόματα. Εάν το ParentProject.CalculationMode είναι Automatic, η μέθοδος επαναπρογραμματίζει αυτόματα όλες τις εργασίες του έργου (ημερομηνίες έναρξης/λήξης, ορίζει πρώιμες/αργότερες ημερομηνίες, υπολογίζει τις καθυστερήσεις, την εργασία και τα πεδία κόστους, επαναϋπολογίζει τα IDs και τα επίπεδα περιγράμματος).

```csharp
public void Add(Task item)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | Εργασία | η καθορισμένη εργασία που θα πρέπει να προστεθεί σε αυτή τη συλλογή εργασιών. |

## Παραδείγματα

Δείχνει πώς να μετακινήσετε μια εργασία κάτω από άλλο γονέα.

```csharp
var project = new Project(DataDir + "MoveTask.mpp") { CalculationMode = CalculationMode.Automatic };

// Get Tasks by Ids
var task = project.RootTask.Children.GetByUid(6);
var task2 = project.RootTask.Children.GetByUid(3);

// Adding Task 6 to another parent
task2.Children.Add(task);
```

### Δείτε επίσης

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add() {#add}

Προσθέτει νέα εργασία στη συλλογή εργασιών του έργου στο ίδιο επίπεδο διάρθρωσης με την τελευταία εργασία.

```csharp
public Task Add()
```

### Τιμή Επιστροφής

επιστρέφει το νεοπροστέθηκε αντικείμενο της κλάσης [`Task`](../../task/).

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

---

## Add(string) {#add_2}

Προσθέτει μια νέα εργασία στη συλλογή υποεργασιών.

```csharp
public Task Add(string taskName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| taskName | String | το καθορισμένο όνομα εργασίας. |

### Τιμή Επιστροφής

επιστρέφει το νεοπροστέθηκε αντικείμενο της κλάσης [`Task`](../../task/).

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

---

## Add(string, int) {#add_3}

Προσθέτει μια νέα επαναλαμβανόμενη εργασία στη συλλογή υποεργασιών.

```csharp
public Task Add(string taskName, int beforeTaskId)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| taskName | String | το καθορισμένο όνομα εργασίας. |
| beforeTaskId | Int32 | Το καθορισμένο id μιας εργασίας πριν από την οποία θα εισαχθεί μια νέα εργασία. |

### Τιμή Επιστροφής

επιστρέφει μια εργασία που εισήχθη πριν από μια εργασία με το καθορισμένο id.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentOutOfRangeException | ArgumentOutOfRangeException εκτοξεύεται εάν το καθορισμένο id δεν είναι έγκυρο id εργασίας. |

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

---

## Add(RecurringTaskParameters) {#add_1}

Εισάγει μια νέα εργασία πριν από μια εργασία με το καθορισμένο id και στο ίδιο επίπεδο διάρθρωσης.

```csharp
public Task Add(RecurringTaskParameters parameters)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| parameters | RecurringTaskParameters | Οι παράμετροι που καθορίζονται για τη δημιουργία επαναλαμβανόμενης εργασίας. |

### Τιμή Επιστροφής

επιστρέφει το νεοπροστέθηκε αντικείμενο της κλάσης [`Task`](../../task/).

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | Εκτοξεύεται εάν οι καθορισμένες παράμετροι είναι null. |
| ArgumentException | Εκτοξεύεται εάν οι καθορισμένες παράμετροι είναι άκυρες. |

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
* class [RecurringTaskParameters](../../recurringtaskparameters/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)


