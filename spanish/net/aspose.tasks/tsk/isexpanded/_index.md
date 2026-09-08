---
title: "Tsk.IsExpanded"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si una tarea resumen está expandida o no en la vista GanttChart"
type: docs
weight: 590
url: /es/net/aspose.tasks/tsk/isexpanded/
---
## Tsk.IsExpanded field

Determina si una tarea de resumen está expandida o no en la vista de GanttChart.

```csharp
public static readonly Key<NullableBool, TaskKey> IsExpanded;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.IsExpanded.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsExpanded, true);

Console.WriteLine("Is Expanded: " + task.Get(Tsk.IsExpanded));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


