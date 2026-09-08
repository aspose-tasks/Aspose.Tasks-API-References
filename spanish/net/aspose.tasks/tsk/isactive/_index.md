---
title: "Tsk.IsActive"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si una tarea está activa. Las tareas inactivas ya no afectan a otras tareas ni al cronograma general del proyecto"
type: docs
weight: 550
url: /es/net/aspose.tasks/tsk/isactive/
---
## Tsk.IsActive field

Determina si una tarea está activa. Las tareas inactivas ya no afectan a otras tareas ni al cronograma general del proyecto.

```csharp
public static readonly Key<NullableBool, TaskKey> IsActive;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.IsActive.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsActive, true);

Console.WriteLine("Is Active: " + task.Get(Tsk.IsActive));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


