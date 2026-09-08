---
title: "Clase TasksReadingException"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.TasksReadingException. Representa el tipo de excepción interna de lectura estándar"
type: docs
weight: 2540
url: /es/net/aspose.tasks/tasksreadingexception/
---
## TasksReadingException class

Representa el tipo de excepción interna de lectura estándar.

```csharp
public class TasksReadingException : TasksLoggedException
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | Obtiene la información de registro de la excepción. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | Obtiene la información de operación de la excepción. |

## Ejemplos

Muestra cómo manejar las excepciones de lectura/escritura del proyecto.

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

### Ver también

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


