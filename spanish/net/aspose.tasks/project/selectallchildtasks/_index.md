---
title: "Project.SelectAllChildTasks"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Project. Recopila recursivamente todas las tareas hijas de la tarea raíz"
type: docs
weight: 1230
url: /es/net/aspose.tasks/project/selectallchildtasks/
---
## Project.SelectAllChildTasks method

Recopila recursivamente todas las tareas hijas de la tarea raíz.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### Valor devuelto

La colección de tareas.

## Ejemplos

Muestra cómo renumerar los códigos WBS de las tareas seleccionadas.

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

var tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// salida: ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode(new List<int> { 1, 2, 3 });

Console.WriteLine("\nWBS codes after: ");

// salida: ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### Ver también

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


