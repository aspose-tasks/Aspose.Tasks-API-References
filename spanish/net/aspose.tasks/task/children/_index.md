---
title: "Task.Children"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Task. Obtiene una colección de tareas hijas de este objeto. Objeto TaskCollection que representa tareas hijas"
type: docs
weight: 190
url: /es/net/aspose.tasks/task/children/
---
## Task.Children property

Obtiene una colección de tareas hijas de este objeto. Objeto TaskCollection que representa tareas hijas.

```csharp
public TaskCollection Children { get; }
```

## Ejemplos

Muestra cómo usar la colección de tareas para agregar una tarea.

```csharp
var project = new Project();

// Agregar tarea, subtarea y guardar proyecto
var task = project.RootTask.Children.Add("Summary1");
task.Children.Add("Subtask1");
project.Save(OutDir + "CreateTasks_out.xml", SaveFileFormat.Xml);
```

### Ver también

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


