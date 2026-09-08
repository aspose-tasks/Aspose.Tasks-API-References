---
title: "Tsk.IsManual"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si una tarea está programada manualmente"
type: docs
weight: 610
url: /es/net/aspose.tasks/tsk/ismanual/
---
## Tsk.IsManual field

Determina si una tarea está programada manualmente.

```csharp
public static readonly Key<NullableBool, TaskKey> IsManual;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.IsManual.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsManual, true);

Console.WriteLine("Is Manual: " + task.Get(Tsk.IsManual));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


