---
title: "Κλάση CheckCircuit"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Util.CheckCircuit κλάση. Ελέγχει ένα δέντρο εργασιών εάν περιέχει κύκλωμα"
type: docs
weight: 2680
url: /el/net/aspose.tasks.util/checkcircuit/
---
## CheckCircuit class

Ελέγχει ένα δέντρο (εργασιών) αν περιέχει κύκλο.

```csharp
public class CheckCircuit : TreeAlgorithmBase<Task>
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [CheckCircuit](checkcircuit/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `CheckCircuit`. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [Alg](../../aspose.tasks.util/checkcircuit/alg/)(Task, int) | Ελέγξτε εάν το καθορισμένο αντικείμενο έχει ήδη επεξεργαστεί. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

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

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


