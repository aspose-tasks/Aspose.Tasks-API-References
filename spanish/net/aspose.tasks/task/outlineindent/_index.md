---
title: "Task.OutlineIndent"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método de Task. Indenta una tarea en el esquema"
type: docs
weight: 1380
url: /es/net/aspose.tasks/task/outlineindent/
---
## Task.OutlineIndent method

Sangra una tarea en el outline.

```csharp
public void OutlineIndent()
```

## Ejemplos

Muestra cómo indentar la tarea.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = project.RootTask.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// indenta la tarea
task2.OutlineIndent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### Ver también

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


