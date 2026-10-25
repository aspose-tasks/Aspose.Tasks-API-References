---
title: "Task.GetHashCode"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método de Task. Devuelve un valor de código hash para esta Task"
type: docs
weight: 1350
url: /es/net/aspose.tasks/task/gethashcode/
---
## Task.GetHashCode method

Devuelve un valor de código hash para este Task.

```csharp
public override int GetHashCode()
```

### Valor devuelto

devuelve un valor de código hash para este objeto.

## Ejemplos

Muestra cómo obtener un código hash de una tarea.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

// el código hash de una tarea se basa en el uid y el nombre de la tarea
Console.WriteLine("Hash code of the task: " + task.GetHashCode());

task.Set(Tsk.Name, "Task 1");

Console.WriteLine("Hash code of the task: " + task.GetHashCode());
```

### Ver también

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


