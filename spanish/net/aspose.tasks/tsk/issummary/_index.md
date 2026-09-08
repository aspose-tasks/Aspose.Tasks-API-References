---
title: "Tsk.IsSummary"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si una tarea es una tarea resumen"
type: docs
weight: 720
url: /es/net/aspose.tasks/tsk/issummary/
---
## Tsk.IsSummary field

Determina si una tarea es una tarea de resumen.

```csharp
public static readonly Key<bool, TaskKey> IsSummary;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.IsSummary.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSummary, true);

Console.WriteLine("Is Summary: " + task.Get(Tsk.IsSummary));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


