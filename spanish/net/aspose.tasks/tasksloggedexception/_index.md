---
title: "Clase TasksLoggedException"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.TasksLoggedException. Representa el tipo de excepción interno estándar"
type: docs
weight: 2530
url: /es/net/aspose.tasks/tasksloggedexception/
---
## TasksLoggedException class

Representa el tipo de excepción interna estándar.

```csharp
public class TasksLoggedException : ApplicationException
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | Obtiene la información de registro de la excepción. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | Obtiene la información de operación de la excepción. |

## Ejemplos

Muestra cómo leer el texto del registro y el tipo de excepción para verificar problemas con la exportación MPP.

```csharp
try
{
    var project = new Project(DataDir + "PrintTaskWritingException.mpp");

    // exporta el proyecto como un archivo MPP
    project.Save(OutDir + "PrintTaskWritingException_out.MPP", SaveFileFormat.Mpp);
}
catch (TasksWritingException ex)
{
    Console.WriteLine("Exception Operation: " + ex.Operation);
    Console.WriteLine("Exception Log Text: ");
    Console.WriteLine(ex.LogText);
}
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


