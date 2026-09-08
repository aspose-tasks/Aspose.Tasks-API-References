---
title: "Clase TasksException"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.TasksException. Representa el tipo de excepción interno estándar"
type: docs
weight: 2520
url: /es/net/aspose.tasks/tasksexception/
---
## TasksException class

Representa el tipo de excepción interna estándar.

```csharp
public class TasksException : ApplicationException
```

## Ejemplos

Muestra cómo detectar la estructura rota del proyecto.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

// verificar la estructura del proyecto.
// Se lanzará el <see cref="TasksException"> si la estructura del proyecto es incorrecta.
try
{
    TaskUtils.Apply(project.RootTask, new CheckCircuit(), 0);
}
catch (TasksException ex)
{
    Console.WriteLine(ex);
}
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


