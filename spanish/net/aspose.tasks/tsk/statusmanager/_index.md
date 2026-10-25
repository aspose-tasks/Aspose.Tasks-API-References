---
title: "Tsk.StatusManager"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El nombre del recurso empresarial que debe recibir actualizaciones de estado para la tarea actual de los recursos"
type: docs
weight: 1050
url: /es/net/aspose.tasks/tsk/statusmanager/
---
## Tsk.StatusManager field

El nombre del recurso empresarial que debe recibir actualizaciones de estado para la tarea actual de los recursos.

```csharp
public static readonly Key<string, TaskKey> StatusManager;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.StatusManager.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StatusManager, "John Smith");

Console.WriteLine("Status Manager: " + task.Get(Tsk.StatusManager));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


