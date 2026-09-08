---
title: "Tsk.IgnoreWarnings"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Indica si se debe ocultar el indicador de advertencia de conflicto de programación en Microsoft Project"
type: docs
weight: 540
url: /es/net/aspose.tasks/tsk/ignorewarnings/
---
## Tsk.IgnoreWarnings field

Indica si se debe ocultar el indicador de advertencia de conflicto de programación en Microsoft Project.

```csharp
public static readonly Key<bool, TaskKey> IgnoreWarnings;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.IgnoreWarnings.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreWarnings, true);

Console.WriteLine("Ignore Warnings: " + task.Get(Tsk.IgnoreWarnings));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


