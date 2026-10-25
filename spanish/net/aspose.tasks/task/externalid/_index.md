---
title: "Task.ExternalId"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Task. Obtiene o establece un valor de ExternalId"
type: docs
weight: 410
url: /es/net/aspose.tasks/task/externalid/
---
## Task.ExternalId property

Obtiene o establece un valor de ExternalId.

```csharp
public int ExternalId { get; set; }
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


