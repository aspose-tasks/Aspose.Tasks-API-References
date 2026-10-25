---
title: "Project.CriticalPath"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Project property. Λαμβάνει μια συλλογή που περιέχει μια λίστα από κρίσιμες εργασίες που αποτελούν το Critical Path αυτού του έργου. Αυτή είναι μια λειτουργία On όπου n είναι ο αριθμός των εργασιών στο έργο."
type: docs
weight: 180
url: /el/net/aspose.tasks/project/criticalpath/
---
## Project.CriticalPath property

Λαμβάνει μια συλλογή που περιέχει μια λίστα από κρίσιμες εργασίες που αποτελούν την Κρίσιμη Διαδρομή αυτού του έργου. Αυτή είναι μια λειτουργία O(n), όπου n είναι ο αριθμός των εργασιών στο έργο.

```csharp
public TaskCollection CriticalPath { get; }
```

### Τιμή Επιστροφής

μια συλλογή που αντιπροσωπεύει μια λίστα όλων των κρίσιμων εργασιών.

## Παραδείγματα

Δείχνει πώς να υπολογίσετε ένα κρίσιμο μονοπάτι του έργου.

```csharp
var project = new Project()
{
    CalculationMode = CalculationMode.Automatic
};

var subtask1 = project.RootTask.Children.Add("1");
var subtask2 = project.RootTask.Children.Add("2");
project.TaskLinks.Add(subtask1, subtask2, TaskLinkType.FinishToStart);

project.RootTask.Children.Add("3");

// Εμφανίστε το κρίσιμο μονοπάτι τώρα
foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id) + "  " + task.Get(Tsk.Name));
    Console.WriteLine(task.Get(Tsk.Start));
    Console.WriteLine(task.Get(Tsk.Finish) + "\n");
}
```

### Δείτε επίσης

* class [TaskCollection](../../taskcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


