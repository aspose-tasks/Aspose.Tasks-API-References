---
title: "Klasse ValidationException"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ValidationException‑klasse. Vertegenwoordigt een uitzondering die wordt gegooid wanneer fouten worden gevonden tijdens de validatie van een entiteit."
type: docs
weight: 2790
url: /nl/net/aspose.tasks/validationexception/
---
## ValidationException class

Stelt een exceptie voor die wordt gegooid wanneer fouten worden gevonden tijdens de validatie van een entiteit.

```csharp
public class ValidationException : ApplicationException
```

## Voorbeelden

Toont hoe &lt;see cref="ValidationException"/&gt; af te handelen tijdens het werken met terugkerende taken.

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

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


