---
title: "TaskLink.CrossProjectName"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad TaskLink. Obtiene o establece el proyecto predecesor externo"
type: docs
weight: 10
url: /es/net/aspose.tasks/tasklink/crossprojectname/
---
## TaskLink.CrossProjectName property

Obtiene o establece el proyecto predecesor externo.

```csharp
public string CrossProjectName { get; set; }
```

## Ejemplos

Muestra cómo encontrar enlaces de tareas entre proyectos.

```csharp
var project = new Project(DataDir + "GetCrossProjectTaskLinks.mpp");

// Verificar enlaces de tareas entre proyectos
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Task Link: " + taskLink.ToString());
    if (taskLink.IsCrossProject)
    {
        Console.WriteLine(taskLink.CrossProjectName);
    }
}
```

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

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


