---
title: "Tsk.HideBar"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si la barra Gantt de una tarea está oculta cuando se muestra en Microsoft Project"
type: docs
weight: 480
url: /es/net/aspose.tasks/tsk/hidebar/
---
## Tsk.HideBar field

Determina si la barra de Gantt de una tarea está oculta al mostrarse en Microsoft Project.

```csharp
public static readonly Key<NullableBool, TaskKey> HideBar;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.HideBar.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.HideBar, true);

Console.WriteLine("Hide Bar: " + task.Get(Tsk.HideBar));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


