---
title: "Κλάση TasksReadingException"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.TasksReadingException. Αντιπροσωπεύει τον τυπικό εσωτερικό τύπο εξαίρεσης ανάγνωσης"
type: docs
weight: 2540
url: /el/net/aspose.tasks/tasksreadingexception/
---
## TasksReadingException class

Αντιπροσωπεύει τον τυπικό εσωτερικό τύπο εξαίρεσης ανάγνωσης.

```csharp
public class TasksReadingException : TasksLoggedException
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | Λαμβάνει τις πληροφορίες καταγραφής της εξαίρεσης. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | Λαμβάνει τις πληροφορίες λειτουργίας της εξαίρεσης. |

## Παραδείγματα

Δείχνει πώς να διαχειριστείτε τις εξαιρέσεις ανάγνωσης/εγγραφής του έργου.

```csharp
try
{
    var project = new Project(DataDir + "project.mpp");
    project.Save(OutDir + "HandleExceptions_out.mpp", SaveFileFormat.Mpp);
}
catch (TasksReadingException ex)
{
    Console.WriteLine("Message: ");
    Console.WriteLine(ex.Message);
    Console.WriteLine("Log: ");
    Console.WriteLine(ex.LogText);
    if (ex.InnerException != null)
    {
        Console.WriteLine("Inner exception message: ");
        Console.WriteLine(ex.InnerException.Message);
    }
}
```

### Δείτε επίσης

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


