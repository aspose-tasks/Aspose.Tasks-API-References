---
title: "TreeAlgorithmBase1.Alg"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "TreeAlgorithmBase μέθοδος. Επεξεργάζεται έναν κόμβο ενός δέντρου"
type: docs
weight: 10
url: /el/net/aspose.tasks.util/treealgorithmbase-1/alg/
---
## TreeAlgorithmBase&lt;T&gt;.Alg method

Επεξεργάζεται έναν κόμβο ενός δέντρου.

```csharp
public abstract void Alg(T el, int level)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | T | Κόμβος προς επεξεργασία. |
| επίπεδο | Int32 | Επίπεδο κόμβου δέντρου. |

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

* class [TreeAlgorithmBase&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../treealgorithmbase-1/)
* assembly [Aspose.Tasks](../../../)


