---
title: "Task.ExternalUid"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad de Task. Obtiene o establece el identificador único de tareas externas cuando la tarea es externa"
type: docs
weight: 430
url: /es/net/aspose.tasks/task/externaluid/
---
## Task.ExternalUid property

Obtiene o establece el identificador único de la tarea externa cuando la tarea es externa.

```csharp
public int ExternalUid { get; set; }
```

## Ejemplos

Muestra cómo crear un enlace de tarea entre proyectos - enlace a una tarea en otro proyecto (externo).

```csharp
Project project = new Project();
var summary = project.RootTask.Children.Add("Summary Task");

// Para crear un enlace a una tarea de otro proyecto debemos crear
// su duplicado (o "externa") tarea en el proyecto actual.

Task t2 = summary.Children.Add("External Task");
t2.Set(Tsk.ExternalTaskProject, "ExternalProject.mpp"); // here we set path to external project's MPP file.
t2.Set(Tsk.ExternalId, 1); // Set External task's Id.
t2.Set(Tsk.ExternalUid, 2); // External task's Unique Id should be set.
t2.Set(Tsk.IsExternalTask, true);
t2.Set(Tsk.IsManual, new NullableBool(false));
t2.Set(Tsk.IsSummary, false);

Task t = summary.Children.Add("Task");
TaskLink link = project.TaskLinks.Add(t2, t);
link.IsCrossProject = true;
link.LinkType = TaskLinkType.FinishToStart;
link.CrossProjectName = "ExternalProject.mpp\\\\1"; // <- here external task's Id is used.
```

### Ver también

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


