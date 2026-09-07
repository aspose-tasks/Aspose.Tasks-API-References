---
title: "Κλάση InvalidPasswordException"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.InvalidPasswordException. Αντιπροσωπεύει τον τύπο εξαίρεσης που ρίχνεται όταν ανοίγεται αρχείο προστατευμένο με κωδικό με λανθασμένο κωδικό."
type: docs
weight: 910
url: /el/net/aspose.tasks/invalidpasswordexception/
---
## InvalidPasswordException class

Αντιπροσωπεύει τον τύπο εξαίρεσης που ρίχνεται όταν ανοίγεται αρχείο προστατευμένο με κωδικό με λανθασμένο κωδικό.

```csharp
public class InvalidPasswordException : TasksException
```

## Παραδείγματα

Δείχνει πώς να χειριστείτε &lt;see cref="InvalidPasswordException"/&gt; κατά την ανάγνωση αρχείων έργου που είναι προστατευμένα με κωδικό.

```csharp
try
{
    var project = new Project(DataDir + "PasswordProtected.mpp");

    // εργασία με το έργο ...
    Console.WriteLine("Project Name: " + project.Get(Prj.Name));
}
catch (TasksReadingException e)
{
    // το μήνυμα είναι "Το έργο είναι προστατευμένο με κωδικό. Ο κωδικός δεν παρέχεται ή είναι λανθασμένος."
    Console.WriteLine(e.Message);
}
```

### Δείτε επίσης

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


