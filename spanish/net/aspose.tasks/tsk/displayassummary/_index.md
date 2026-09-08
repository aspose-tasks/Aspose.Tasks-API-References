---
title: "Tsk.DisplayAsSummary"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si la tarea debe mostrarse como una tarea resumen. La lectura solo es compatible con el formato XML"
type: docs
weight: 280
url: /es/net/aspose.tasks/tsk/displayassummary/
---
## Tsk.DisplayAsSummary field

Determina si la tarea debe mostrarse como una tarea resumen. Lectura compatible solo con formato XML.

```csharp
public static readonly Key<NullableBool, TaskKey> DisplayAsSummary;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.DisplayAsSummary.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayAsSummary, true);

Console.WriteLine("Display As Summary: " + task.Get(Tsk.DisplayAsSummary));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


