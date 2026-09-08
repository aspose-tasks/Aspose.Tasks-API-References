---
title: "Tsk.IsSubproject"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si una tarea es un proyecto insertado"
type: docs
weight: 700
url: /es/net/aspose.tasks/tsk/issubproject/
---
## Tsk.IsSubproject field

Determina si una tarea es un proyecto insertado.

```csharp
public static readonly Key<bool, TaskKey> IsSubproject;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.IsSubproject.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSubproject, true);

Console.WriteLine("Is Subproject: " + task.Get(Tsk.IsSubproject));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


