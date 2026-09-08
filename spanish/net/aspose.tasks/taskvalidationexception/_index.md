---
title: "Clase TaskValidationException"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.TaskValidationException. Representa una excepción que se lanza cuando se encuentran errores en las tareas del proyecto después de la recalculación"
type: docs
weight: 2510
url: /es/net/aspose.tasks/taskvalidationexception/
---
## TaskValidationException class

Representa una excepción que se lanza cuando se encuentran errores en las tareas del proyecto después de la recalculación.

```csharp
public class TaskValidationException : RecalculationValidationException
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Task](../../aspose.tasks/taskvalidationexception/task/) { get; } | Obtiene la tarea que causó la excepción. |

## Ejemplos

Muestra bajo qué condiciones la excepción &lt;see cref="TaskValidationException" /&gt; puede ser lanzada.

```csharp
try
{
    var project = new Project { CalculationMode = CalculationMode.None };
    var task = project.RootTask.Children.Add("Task");

    // establecer fechas incorrectas accidentalmente
    task.Set(Tsk.Start, new DateTime(2017, 6, 19, 8, 0, 0));
    task.Set(Tsk.Duration, project.GetDuration(1));
    task.Set(Tsk.Finish, new DateTime(2017, 6, 18, 17, 0, 0));

    // ejecutar la recalculación del proyecto con una bandera para ejecutar la validación
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Ver también

* class [RecalculationValidationException](../recalculationvalidationexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


