---
title: "TasksLoggedException.LogText"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα TasksLoggedException. Λαμβάνει τις πληροφορίες καταγραφής της εξαίρεσης"
type: docs
weight: 10
url: /el/net/aspose.tasks/tasksloggedexception/logtext/
---
## TasksLoggedException.LogText property

Λαμβάνει τις πληροφορίες καταγραφής της εξαίρεσης.

```csharp
public string LogText { get; }
```

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

* class [TasksLoggedException](../)
* namespace [Aspose.Tasks](../../tasksloggedexception/)
* assembly [Aspose.Tasks](../../../)


