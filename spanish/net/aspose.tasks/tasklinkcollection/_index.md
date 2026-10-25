---
title: "Clase TaskLinkCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.TaskLinkCollection clase. Representa una colección de objetos Task."
type: docs
weight: 2420
url: /es/net/aspose.tasks/tasklinkcollection/
---
## TaskLinkCollection class

Representa una colección de [`Task`](../task/) objetos.

```csharp
public class TaskLinkCollection : IList<TaskLink>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/tasklinkcollection/count/) { get; } | Obtiene el número de objetos contenidos en este objeto `TaskLinkCollection`. |
| [Item](../../aspose.tasks/tasklinkcollection/item/) { get; set; } | Devuelve o establece el elemento en el índice especificado. |
| [ParentProject](../../aspose.tasks/tasklinkcollection/parentproject/) { get; } | Obtiene el proyecto principal del objeto ResourceAssignmentCollection. Proyecto padre [`Project`](../project/) para este objeto. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_3)(TaskLink) | Esta es la implementación de referencia del método Add de ICollection, que solo lanza NotSupportedException |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add)(Task, Task) | Devuelve una instancia de Finish-Start [`TaskLink`](../tasklink/) que ha sido añadida al objeto TaskLinkCollection. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_1)(Task, Task, TaskLinkType) | Devuelve una instancia de [`TaskLink`](../tasklink/) que ha sido añadida al objeto TaskLinkCollection. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_2)(Task, Task, TaskLinkType, Duration) | Devuelve una instancia de [`TaskLink`](../tasklink/) que ha sido añadida al objeto TaskLinkCollection. |
| [GetEnumerator](../../aspose.tasks/tasklinkcollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [Remove](../../aspose.tasks/tasklinkcollection/remove/)(TaskLink) | Elimina el enlace de tarea de un proyecto. |
| [ToList](../../aspose.tasks/tasklinkcollection/tolist/)() | Convierte el objeto TaskLinkCollection en una lista de objetos [`TaskLink`](../tasklink/). |

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

* class [TaskLink](../tasklink/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


