---
title: "Tsk.Guid"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Los códigos de identificación únicos generados para una tarea."
type: docs
weight: 460
url: /es/net/aspose.tasks/tsk/guid/
---
## Tsk.Guid field

Los códigos de identificación únicos generados para una tarea.

```csharp
public static readonly Key<string, TaskKey> Guid;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.Guid.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Guid, "60648d59-9c2b-4dc6-bfdb-bfd38f331d61");

Console.WriteLine("Guid: " + task.Get(Tsk.Guid));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


