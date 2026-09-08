---
title: "TaskLinkCollection.Add"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método TaskLinkCollection. Devuelve una instancia de FinishStart TaskLink que ha sido añadida al objeto TaskLinkCollection"
type: docs
weight: 40
url: /es/net/aspose.tasks/tasklinkcollection/add/
---
## Add(Task, Task) {#add}

Devuelve una instancia de Finish-Start [`TaskLink`](../../tasklink/) que se ha añadido al objeto TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pred | Tarea | Tarea predecesora. |
| succ | Tarea | Tarea sucesora. |

### Valor devuelto

una instancia de enlace de tarea que se ha añadido a este objeto.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | Si alguna de las tareas de entrada es nula, se lanzará ArgumentNullException. |

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
* class [Task](../../task/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType) {#add_1}

Devuelve una instancia de [`TaskLink`](../../tasklink/) que se ha añadido al objeto TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pred | Tarea | Tarea predecesora. |
| succ | Tarea | Tarea sucesora. |
| linkType | TaskLinkType | Tipo de enlace [`TaskLinkType`](../../tasklinktype/) |

### Valor devuelto

una instancia de enlace de tarea que se ha añadido a este objeto.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | Si alguna de las tareas de entrada es nula, se lanzará ArgumentNullException. |

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
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType, Duration) {#add_2}

Devuelve una instancia de [`TaskLink`](../../tasklink/) que se ha añadido al objeto TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType, Duration lag)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pred | Tarea | Tarea predecesora. |
| succ | Tarea | Tarea sucesora. |
| linkType | TaskLinkType | Tipo de enlace [`TaskLinkType`](../../tasklinktype/) |
| lag | Duration | Retardo del enlace [`Duration`](../../duration/). |

### Valor devuelto

un enlace de tarea que se ha añadido a este objeto.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | Si alguna de las tareas de entrada es nula, se lanzará ArgumentNullException. |

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
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* struct [Duration](../../duration/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(TaskLink) {#add_3}

Esta es la implementación de referencia del método Add de ICollection, que solo lanza NotSupportedException

```csharp
public void Add(TaskLink item)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| elemento | TaskLink | El elemento a añadir. |

### Ver también

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


