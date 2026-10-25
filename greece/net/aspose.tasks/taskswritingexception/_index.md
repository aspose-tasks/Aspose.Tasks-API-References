---
title: "Κλάση TasksWritingException"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.TasksWritingException κλάση. Αντιπροσωπεύει τον τυπικό εσωτερικό τύπο εξαίρεσης εγγραφής"
type: docs
weight: 2560
url: /el/net/aspose.tasks/taskswritingexception/
---
## TasksWritingException class

Αντιπροσωπεύει τον τυπικό εσωτερικό τύπο εξαίρεσης εγγραφής.

```csharp
public class TasksWritingException : TasksLoggedException
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | Λαμβάνει τις πληροφορίες καταγραφής της εξαίρεσης. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | Λαμβάνει τις πληροφορίες λειτουργίας της εξαίρεσης. |

## Παραδείγματα

Δείχνει πώς να διαβάσετε το κείμενο καταγραφής και τον τύπο της εξαίρεσης για να ελέγξετε προβλήματα με την εξαγωγή MPP.

```csharp
try
{
    var project = new Project(DataDir + "PrintTaskWritingException.mpp");

    // εξάγετε το έργο ως αρχείο MPP
    project.Save(OutDir + "PrintTaskWritingException_out.MPP", SaveFileFormat.Mpp);
}
catch (TasksWritingException ex)
{
    Console.WriteLine("Exception Operation: " + ex.Operation);
    Console.WriteLine("Exception Log Text: ");
    Console.WriteLine(ex.LogText);
}
```

### Δείτε επίσης

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


