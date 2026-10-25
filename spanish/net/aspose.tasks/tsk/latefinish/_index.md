---
title: "Tsk.LateFinish"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. La fecha más reciente en que una tarea puede terminar sin retrasar la finalización del proyecto"
type: docs
weight: 730
url: /es/net/aspose.tasks/tsk/latefinish/
---
## Tsk.LateFinish field

La fecha más reciente en que una tarea puede finalizar sin retrasar la finalización del proyecto.

```csharp
public static readonly Key<DateTime, TaskKey> LateFinish;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.LateFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Finish: " + task.Get(Tsk.LateFinish));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


