---
title: "TaskUtils.TaskChildrenCount"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método TaskUtils. Calcula recursivamente el número de tareas hijas a través de todos los niveles"
type: docs
weight: 40
url: /es/net/aspose.tasks.util/taskutils/taskchildrencount/
---
## TaskUtils.TaskChildrenCount method

Calcula recursivamente el número de tareas hijas de una tarea a través de todos los niveles.

```csharp
public static int TaskChildrenCount(Task task)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tarea | Tarea | La tarea cuyos hijos se calculan. |

### Valor devuelto

El número de hijos.

## Ejemplos

Muestra cómo usar &lt;see cref="Aspose.Tasks.Util.TaskUtils.TaskChildrenCount" /&gt; método.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// calcula recursivamente el número de tareas hijas de la tarea a través de todos los niveles
var count = TaskUtils.TaskChildrenCount(project.RootTask);

Console.WriteLine("Number of tasks: " + count);
```

### Ver también

* class [Task](../../../aspose.tasks/task/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


