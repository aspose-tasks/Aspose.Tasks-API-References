---
title: "Task.OutlineIndent"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Task. Εσοπίζει μια εργασία στο διάγραμμα"
type: docs
weight: 1380
url: /el/net/aspose.tasks/task/outlineindent/
---
## Task.OutlineIndent method

Αυξάνει την εσοχή μιας εργασίας στο περίγραμμα.

```csharp
public void OutlineIndent()
```

## Παραδείγματα

Δείχνει πώς να εσοπίσετε μια εργασία.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = project.RootTask.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// εσοπίστε την εργασία
task2.OutlineIndent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### Δείτε επίσης

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


