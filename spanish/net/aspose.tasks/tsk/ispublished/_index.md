---
title: "Tsk.IsPublished"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si la tarea actual debe publicarse en Project Server junto con el resto del proyecto"
type: docs
weight: 660
url: /es/net/aspose.tasks/tsk/ispublished/
---
## Tsk.IsPublished field

Determina si la tarea actual debe publicarse en Project Server junto con el resto del proyecto.

```csharp
public static readonly Key<NullableBool, TaskKey> IsPublished;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.IsPublished.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsPublished, true);

Console.WriteLine("Is Published: " + task.Get(Tsk.IsPublished));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


