---
title: "Clase ValidationException"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.ValidationException. Representa una excepción que se lanza cuando se encuentran errores durante la validación de la entidad."
type: docs
weight: 2790
url: /es/net/aspose.tasks/validationexception/
---
## ValidationException class

Representa una excepción que se lanza cuando se encuentran errores durante la validación de la entidad.

```csharp
public class ValidationException : ApplicationException
```

## Ejemplos

Muestra cómo manejar &lt;see cref="ValidationException"/&gt; mientras se trabaja con tareas recurrentes.

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

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


