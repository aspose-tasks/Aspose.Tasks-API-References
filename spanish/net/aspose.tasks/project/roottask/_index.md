---
title: "Project.RootTask"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Project. Obtiene la raíz del árbol de tareas"
type: docs
weight: 800
url: /es/net/aspose.tasks/project/roottask/
---
## Project.RootTask property

Obtiene la raíz del árbol de tareas.

```csharp
public Task RootTask { get; }
```

## Ejemplos

Muestra cómo agregar una tarea a un proyecto usando la tarea raíz del proyecto.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddNewTask_out.xml", SaveFileFormat.Xml);
```

### Ver también

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


