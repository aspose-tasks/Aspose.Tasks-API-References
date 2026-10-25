---
title: "Κλάση TaskValidationException"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.TaskValidationException. Αντιπροσωπεύει μια εξαίρεση που ρίχνεται όταν εντοπίζονται σφάλματα στις εργασίες των έργων μετά την επανυπολογισμό"
type: docs
weight: 2510
url: /el/net/aspose.tasks/taskvalidationexception/
---
## TaskValidationException class

Αντιπροσωπεύει μια εξαίρεση που ρίχνεται όταν εντοπιστούν σφάλματα στις εργασίες του έργου μετά την επανυπολογισμό.

```csharp
public class TaskValidationException : RecalculationValidationException
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Task](../../aspose.tasks/taskvalidationexception/task/) { get; } | Παίρνει την εργασία που προκάλεσε την εξαίρεση. |

## Παραδείγματα

Δείχνει υπό ποιες συνθήκες μπορεί να ριχθεί η εξαίρεση &lt;see cref="TaskValidationException" /&gt;.

```csharp
try
{
    var project = new Project { CalculationMode = CalculationMode.None };
    var task = project.RootTask.Children.Add("Task");

    // κατά λάθος ορίσατε λανθασμένες ημερομηνίες
    task.Set(Tsk.Start, new DateTime(2017, 6, 19, 8, 0, 0));
    task.Set(Tsk.Duration, project.GetDuration(1));
    task.Set(Tsk.Finish, new DateTime(2017, 6, 18, 17, 0, 0));

    // εκτελέστε επανυπολογισμό του έργου με μια σημαία για εκτέλεση επικύρωσης
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Δείτε επίσης

* class [RecalculationValidationException](../recalculationvalidationexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


