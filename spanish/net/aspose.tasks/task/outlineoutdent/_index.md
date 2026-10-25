---
title: "Task.OutlineOutdent"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método de Task. Promueve una tarea en el esquema"
type: docs
weight: 1390
url: /es/net/aspose.tasks/task/outlineoutdent/
---
## Task.OutlineOutdent method

Promueve una tarea en el outline.

```csharp
public void OutlineOutdent()
```

## Ejemplos

Muestra cómo desidentar una tarea.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = task1.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// desidentar la tarea
task2.OutlineOutdent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### Ver también

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


