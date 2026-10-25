---
title: "Task.Delete"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Task. Διαγράφει μια εργασία από τη συλλογή εργασιών του γονικού έργου και όλες τις αναθέσεις της."
type: docs
weight: 1320
url: /el/net/aspose.tasks/task/delete/
---
## Task.Delete method

Διαγράφει μια εργασία από τη συλλογή εργασιών του γονικού έργου και όλες τις αναθέσεις της.

```csharp
public void Delete()
```

## Παραδείγματα

Δείχνει πώς να διαγράψετε μια εργασία.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);

// διαγράψτε μια εργασία
task.Delete();

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);
```

### Δείτε επίσης

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


