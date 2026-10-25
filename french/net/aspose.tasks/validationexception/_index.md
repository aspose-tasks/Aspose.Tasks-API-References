---
title: "Classe ValidationException"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.ValidationException. Représente une exception qui est levée lorsque des erreurs sont détectées lors de la validation de l'entité."
type: docs
weight: 2790
url: /fr/net/aspose.tasks/validationexception/
---
## ValidationException class

Représente une exception qui est levée lorsque des erreurs sont détectées lors de la validation de l'entité.

```csharp
public class ValidationException : ApplicationException
```

## Exemples

Montre comment gérer &lt;see cref="ValidationException"/&gt; lors du travail avec des tâches récurrentes.

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

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


