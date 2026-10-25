---
title: "Project.CalculationMode"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Project. Λαμβάνει ή ορίζει τη λειτουργία υπολογισμού ενός έργου. Μπορεί να είναι μία από τις τιμές της απαρίθμησης CalculationMode"
type: docs
weight: 110
url: /el/net/aspose.tasks/project/calculationmode/
---
## Project.CalculationMode property

Λαμβάνει ή ορίζει τη λειτουργία υπολογισμού ενός έργου. Μπορεί να είναι μία από τις τιμές της απαρίθμησης `CalculationMode`.

```csharp
public CalculationMode CalculationMode { get; set; }
```

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τη λειτουργία υπολογισμού του έργου.

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

* enum [CalculationMode](../../calculationmode/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


