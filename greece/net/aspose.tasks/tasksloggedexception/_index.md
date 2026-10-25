---
title: "Κλάση TasksLoggedException"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Η κλάση Aspose.Tasks.TasksLoggedException. Αντιπροσωπεύει τον τυπικό εσωτερικό τύπο εξαίρεσης"
type: docs
weight: 2530
url: /el/net/aspose.tasks/tasksloggedexception/
---
## TasksLoggedException class

Αντιπροσωπεύει τον τυπικό εσωτερικό τύπο εξαίρεσης.

```csharp
public class TasksLoggedException : ApplicationException
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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


