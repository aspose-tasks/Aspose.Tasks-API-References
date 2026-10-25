---
title: "Tsk.DisplayOnTimeline"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Especifica si una tarea debe mostrarse en una vista de línea de tiempo"
type: docs
weight: 290
url: /es/net/aspose.tasks/tsk/displayontimeline/
---
## Tsk.DisplayOnTimeline field

Especifica si una tarea debe mostrarse en una vista de línea de tiempo.

```csharp
public static readonly Key<bool, TaskKey> DisplayOnTimeline;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.DisplayOnTimeline.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayOnTimeline, true);

Console.WriteLine("Display On Timeline: " + task.Get(Tsk.DisplayOnTimeline));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


