---
title: "Κλάση TasksException"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.TasksException. Αντιπροσωπεύει τον τυπικό εσωτερικό τύπο εξαίρεσης"
type: docs
weight: 2520
url: /el/net/aspose.tasks/tasksexception/
---
## TasksException class

Αντιπροσωπεύει τον τυπικό εσωτερικό τύπο εξαίρεσης.

```csharp
public class TasksException : ApplicationException
```

## Παραδείγματα

Δείχνει πώς να εντοπίσετε τη σπασμένη δομή του έργου.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

// ελέγξτε τη δομή του έργου.
// Η <see cref="TasksException"> θα εξαχθεί εάν η δομή του έργου είναι εσφαλμένη.
try
{
    TaskUtils.Apply(project.RootTask, new CheckCircuit(), 0);
}
catch (TasksException ex)
{
    Console.WriteLine(ex);
}
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


