---
title: "Απαρίθμηση CalculationMode"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.CalculationMode. Καθορίζει τη λειτουργία υπολογισμού του έργου"
type: docs
weight: 210
url: /el/net/aspose.tasks/calculationmode/
---
## CalculationMode enumeration

Καθορίζει τη λειτουργία υπολογισμού του έργου.

```csharp
public enum CalculationMode
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| None | `0` | None. Οι ημερομηνίες και τα κόστη του έργου δεν επαναϋπολογίζονται σε αυτή τη λειτουργία. |
| Automatic | `1` | Αυτόματη λειτουργία. Οι ημερομηνίες και τα κόστη του έργου επαναϋπολογίζονται όταν χρησιμοποιείται αυτή η λειτουργία. |
| Manual | `2` | Χειροκίνητη λειτουργία. Μόνο τα απαραίτητα πεδία επαναϋπολογίζονται σε αυτή τη λειτουργία, για παράδειγμα τα UID και τα ID των αντικειμένων. |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τη λειτουργία αυτόματου υπολογισμού.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Automatic
};

// Ορίστε την ημερομηνία έναρξης του έργου και προσθέστε νέες εργασίες
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// Συνδέστε εργασίες
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// Επαληθεύστε ότι οι ημερομηνίες έχουν επαναϋπολογιστεί
Console.WriteLine("Task1 Start + 1 Equals Task2 Start : {0} ", task1.Get(Tsk.Start).AddDays(1).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish + 1 Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).AddDays(1).Equals(task2.Get(Tsk.Finish)));
Console.WriteLine("RootTask Finish Equals Task2 Finish : {0} ", task2.Get(Tsk.Finish).Equals(project.RootTask.Get(Tsk.Finish)));
Console.WriteLine("Project Finish Date Equals Task2 Finish : {0} ", task2.Get(Tsk.Finish).Equals(project.Get(Prj.FinishDate)));
```

Δείχνει πώς να χρησιμοποιήσετε τη λειτουργία none.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.None
};

// Προσθέστε μια νέα εργασία
var task = project.RootTask.Children.Add("Task");

// Σημειώστε ότι ακόμη και τα ids δεν υπολογίστηκαν            
Console.WriteLine("Task.Id Equals 0 : {0} ", task.Get(Tsk.Id).Equals(0));
Console.WriteLine("Task.OutlineLevel Equals 0 : {0} ", task.Get(Tsk.OutlineLevel).Equals(0));
Console.WriteLine("Task Start Equals DateTime.MinValue : {0} ", task.Get(Tsk.Start).Equals(DateTime.MinValue));
Console.WriteLine("Task Finish Equals DateTime.MinValue : {0} ", task.Get(Tsk.Finish).Equals(DateTime.MinValue));
Console.WriteLine("Task Duration Equals 0 mins : {0} ", task.Get(Tsk.Duration).ToString().Equals("0 mins"));

// Ορίστε την ιδιότητα duration
task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));
Console.WriteLine("Task Duration Equals 2 days : {0} ", task.Get(Tsk.Duration).ToString().Equals("2 days"));
Console.WriteLine("Task Start Equals DateTime.MinValue  : {0} ", task.Get(Tsk.Start).Equals(DateTime.MinValue));
Console.WriteLine("Task Finish Equals DateTime.MinValue  : {0} ", task.Get(Tsk.Finish).Equals(DateTime.MinValue));
```

Δείχνει πώς να χρησιμοποιήσετε τη λειτουργία manual calculation mode.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Manual
};

// Ορίστε την ημερομηνία έναρξης του έργου και προσθέστε νέες εργασίες
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// Οι απαραίτητες ιδιότητες ορίζονται σε manual mode
Console.WriteLine("Task1.Id Equals 1 : {0} ", task1.Get(Tsk.Id).Equals(1));
Console.WriteLine("Task1 OutlineLevel Equals 1 : {0} ", task1.Get(Tsk.OutlineLevel).Equals(1));
Console.WriteLine("Task1 Start Equals 15/04/2015 08:00 AM : {0} ", task1.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task1 Finish Equals 15/04/2015 05:00 PM : {0} ", task1.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task1 Duration Equals 1 day : {0} ", task1.Get(Tsk.Duration).ToString().Equals("1 day"));
Console.WriteLine("Task2 Start Equals 15/04/2015 08:00 AM : {0} ", task2.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task2 Finish Equals 15/04/2015 05:00 PM : {0} ", task2.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task2 Duration Equals 1 day : {0} ", task2.Get(Tsk.Duration).ToString().Equals("1 day"));

// Όταν συνδέουμε δύο εργασίες μαζί, οι ημερομηνίες τους δεν επαναϋπολογίζονται σε manual mode
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// Η έναρξη Task 2 δεν έχει αλλάξει
Console.WriteLine("Task1 Start Equals Task2 Start : {0} ", task1.Get(Tsk.Start).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).Equals(task2.Get(Tsk.Finish)));
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


