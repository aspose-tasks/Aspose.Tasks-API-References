---
title: "Κλάση ValidationException"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.ValidationException. Αντιπροσωπεύει μια εξαίρεση που ρίχνεται όταν εντοπίζονται σφάλματα κατά την επικύρωση της οντότητας."
type: docs
weight: 2790
url: /el/net/aspose.tasks/validationexception/
---
## ValidationException class

Αντιπροσωπεύει μια εξαίρεση που ρίχνεται όταν εντοπιστούν σφάλματα κατά την επικύρωση της οντότητας.

```csharp
public class ValidationException : ApplicationException
```

## Παραδείγματα

Δείχνει πώς να χειριστείτε το &lt;see cref=\"ValidationException\"/&gt; ενώ εργάζεστε με επαναλαμβανόμενες εργασίες.

```csharp
try
{
    var project = new Project();
    var parameters = new RecurringTaskParameters { TaskName = "t1", Duration = project.GetDuration(1, TimeUnitType.Day), RecurrencePattern = null };
    project.RootTask.Children.Add(parameters);
}
catch (ValidationException ex)
{
    Console.WriteLine("Message: ");
    Console.WriteLine(ex.Message);
    if (ex.InnerException != null)
    {
        Console.WriteLine("Inner exception message: ");
        Console.WriteLine(ex.InnerException.Message);
    }
}
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


