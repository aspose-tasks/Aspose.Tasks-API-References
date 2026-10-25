---
title: "CheckCircuit.Alg"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος CheckCircuit. Ελέγχει εάν το καθορισμένο αντικείμενο έχει ήδη επεξεργαστεί"
type: docs
weight: 20
url: /el/net/aspose.tasks.util/checkcircuit/alg/
---
## CheckCircuit.Alg method

Ελέγξτε εάν το καθορισμένο αντικείμενο έχει ήδη επεξεργαστεί.

```csharp
public override void Alg(Task el, int level)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| el | Εργασία | Αντικείμενο προς επεξεργασία. |
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

* class [Task](../../../aspose.tasks/task/)
* class [CheckCircuit](../)
* namespace [Aspose.Tasks.Util](../../checkcircuit/)
* assembly [Aspose.Tasks](../../../)


