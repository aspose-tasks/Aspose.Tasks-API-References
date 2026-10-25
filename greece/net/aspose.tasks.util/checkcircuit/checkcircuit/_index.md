---
title: "CheckCircuit.CheckCircuit"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής CheckCircuit. Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης CheckCircuit"
type: docs
weight: 10
url: /el/net/aspose.tasks.util/checkcircuit/checkcircuit/
---
## CheckCircuit constructor

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`CheckCircuit`](../).

```csharp
public CheckCircuit()
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

* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


