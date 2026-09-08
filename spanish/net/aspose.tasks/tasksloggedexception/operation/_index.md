---
title: "TasksLoggedException.Operation"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "propiedad TasksLoggedException. Obtiene la información de la operación de la excepción"
type: docs
weight: 20
url: /es/net/aspose.tasks/tasksloggedexception/operation/
---
## TasksLoggedException.Operation property

Obtiene la información de operación de la excepción.

```csharp
public string Operation { get; }
```

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

* class [TasksLoggedException](../)
* namespace [Aspose.Tasks](../../tasksloggedexception/)
* assembly [Aspose.Tasks](../../../)


