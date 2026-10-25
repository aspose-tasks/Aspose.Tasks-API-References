---
title: "Tsk.IsNull"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si una tarea es una tarea nula"
type: docs
weight: 640
url: /es/net/aspose.tasks/tsk/isnull/
---
## Tsk.IsNull field

Determina si una tarea es una tarea nula.

```csharp
public static readonly Key<NullableBool, TaskKey> IsNull;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.IsNull.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsNull, true);

Console.WriteLine("Is Null: " + task.Get(Tsk.IsNull));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


