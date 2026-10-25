---
title: "TaskLinkCollection.ToList"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método TaskLinkCollection. Convierte el objeto TaskLinkCollection en una lista de objetos TaskLink"
type: docs
weight: 70
url: /es/net/aspose.tasks/tasklinkcollection/tolist/
---
## TaskLinkCollection.ToList method

Convierte el objeto TaskLinkCollection en una lista de objetos [`TaskLink`](../../tasklink/).

```csharp
public List<TaskLink> ToList()
```

### Valor devuelto

Lista de objetos [`TaskLink`](../../tasklink/).

## Ejemplos

Muestra cómo trabajar con colecciones de enlaces de tarea.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// obtener tareas
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// enlazar las tareas
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// imprimir enlaces entre las tareas
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// editar enlace mediante acceso por índice
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// eliminar todos los enlaces de tarea
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### Ver también

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


