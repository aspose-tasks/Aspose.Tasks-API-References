---
title: "Classe ValidationException"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.ValidationException. Rappresenta un'eccezione che viene generata quando vengono trovati errori durante la convalida dell'entità"
type: docs
weight: 2790
url: /it/net/aspose.tasks/validationexception/
---
## ValidationException class

Rappresenta un'eccezione che viene lanciata quando vengono trovati errori durante la convalida dell'entità.

```csharp
public class ValidationException : ApplicationException
```

## Esempi

Mostra come gestire &lt;see cref="ValidationException"/&gt; durante il lavoro con attività ricorrenti.

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

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


