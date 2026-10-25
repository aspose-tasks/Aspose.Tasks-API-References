---
title: "Enumeración TaskLinkType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.TaskLinkType. Especifica el tipo de dependencia de tareas."
type: docs
weight: 2440
url: /es/net/aspose.tasks/tasklinktype/
---
## TaskLinkType enumeration

Especifica el tipo de dependencia de tareas.

```csharp
public enum TaskLinkType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| FinishToFinish | `0` | Relación Fin-Fin |
| FinishToStart | `1` | Relación Fin-Inicio |
| StartToFinish | `2` | Relación Inicio-Fin |
| StartToStart | `3` | Relación Inicio-Inicio |

## Ejemplos

Muestra cómo obtener/establecer un tipo de enlace de un vínculo de tarea.

```csharp
var project = new Project();

// Agregar nuevas tareas
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// Vincular tareas con el tipo de enlace establecido en Inicio a Inicio
var newLink = project.TaskLinks.Add(pred, succ);
newLink.LinkType = TaskLinkType.StartToStart;

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Task Link Type: " + link.LinkType.ToString());
}
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


