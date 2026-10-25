---
title: "Class RecalculationValidationException"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.RecalculationValidationException class. Αντιπροσωπεύει μια εξαίρεση που ρίχνεται όταν εντοπίζονται σφάλματα στο έργο μετά την επανυπολογισμό"
type: docs
weight: 1680
url: /el/net/aspose.tasks/recalculationvalidationexception/
---
## RecalculationValidationException class

Αντιπροσωπεύει μια εξαίρεση που ρίχνεται όταν εντοπίζονται σφάλματα στο έργο μετά από επανυπολογισμό.

```csharp
public abstract class RecalculationValidationException : ValidationException
```

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

* class [ValidationException](../validationexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


