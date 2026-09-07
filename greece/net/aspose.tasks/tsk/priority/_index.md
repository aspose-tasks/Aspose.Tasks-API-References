---
title: "Tsk.Priority"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Το επίπεδο σημασίας που δίνεται σε μια εργασία, το οποίο με τη σειρά του υποδεικνύει πόσο εύκολα μια εργασία ή ανάθεση μπορεί να καθυστερήσει ή να χωριστεί κατά τη βελτιστοποίηση πόρων."
type: docs
weight: 930
url: /el/net/aspose.tasks/tsk/priority/
---
## Tsk.Priority field

Το επίπεδο σημασίας που δίνεται σε μια εργασία, το οποίο με τη σειρά του υποδεικνύει πόσο εύκολα μια εργασία ή ανάθεση μπορεί να καθυστερήσει ή να χωριστεί κατά τη διάρκεια της εξισορρόπησης πόρων.

```csharp
public static readonly Key<int, TaskKey> Priority;
```

## Παραδείγματα

Εμφανίζει πώς να διαβάσετε την προτεραιότητα μιας εργασίας.

```csharp
var project = new Project(DataDir + "TaskPriority.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Εμφάνιση προτεραιοτήτων για όλες τις εργασίες
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Priority : " + task.Get(Tsk.Priority));
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


