---
title: "Project.SelectAllChildTasks"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Project. Συλλέγει επαναληπτικά όλες τις υποεργασίες της ριζικής εργασίας."
type: docs
weight: 1230
url: /el/net/aspose.tasks/project/selectallchildtasks/
---
## Project.SelectAllChildTasks method

Συλλέγει αναδρομικά όλες τις θυγατρικές εργασίες της ριζικής εργασίας.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### Τιμή Επιστροφής

Η συλλογή των εργασιών.

## Παραδείγματα

Δείχνει πώς να επανααριθμήσετε τους κωδικούς WBS των επιλεγμένων εργασιών.

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

var tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// έξοδος: ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode(new List<int> { 1, 2, 3 });

Console.WriteLine("\nWBS codes after: ");

// έξοδος: ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### Δείτε επίσης

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


