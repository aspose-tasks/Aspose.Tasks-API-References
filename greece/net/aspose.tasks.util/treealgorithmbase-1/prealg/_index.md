---
title: "TreeAlgorithmBase1.PreAlg"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "TreeAlgorithmBase μέθοδος. Καλείται πριν από την επεξεργασία ενός κόμβου ενός δέντρου"
type: docs
weight: 30
url: /el/net/aspose.tasks.util/treealgorithmbase-1/prealg/
---
## TreeAlgorithmBase&lt;T&gt;.PreAlg method

Καλείται πριν από την επεξεργασία ενός κόμβου ενός δέντρου.

```csharp
public virtual void PreAlg(T el, int level)
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


