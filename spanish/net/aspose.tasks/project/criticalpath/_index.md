---
title: "Project.CriticalPath"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad de Project. Obtiene una colección que contiene una lista de tareas Critical que componen la ruta crítica de este proyecto. Esta es una operación On donde n es el número de tareas en el proyecto."
type: docs
weight: 180
url: /es/net/aspose.tasks/project/criticalpath/
---
## Project.CriticalPath property

Obtiene una colección que contiene una lista de tareas Critical que forman la ruta crítica de este proyecto. Esta es una operación O(n), donde n es el número de tareas del proyecto.

```csharp
public TaskCollection CriticalPath { get; }
```

### Valor devuelto

una colección que representa una lista de todas las tareas críticas.

## Ejemplos

Muestra cómo calcular la ruta crítica del proyecto.

```csharp
var project = new Project()
{
    CalculationMode = CalculationMode.Automatic
};

var subtask1 = project.RootTask.Children.Add("1");
var subtask2 = project.RootTask.Children.Add("2");
project.TaskLinks.Add(subtask1, subtask2, TaskLinkType.FinishToStart);

project.RootTask.Children.Add("3");

// Muestra la ruta crítica ahora
foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id) + "  " + task.Get(Tsk.Name));
    Console.WriteLine(task.Get(Tsk.Start));
    Console.WriteLine(task.Get(Tsk.Finish) + "\n");
}
```

### Ver también

* class [TaskCollection](../../taskcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


