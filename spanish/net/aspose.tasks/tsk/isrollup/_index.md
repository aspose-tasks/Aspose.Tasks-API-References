---
title: "Tsk.IsRollup"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina si la información sobre las barras Gantt de la subtarea se consolidará en la barra de la tarea resumida."
type: docs
weight: 690
url: /es/net/aspose.tasks/tsk/isrollup/
---
## Tsk.IsRollup field

Determina si la información sobre las barras de Gantt de la subtarea se consolidará en la barra de la tarea de resumen.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRollup;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.IsRollup.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRollup, true);

Console.WriteLine("Is Rollup: " + task.Get(Tsk.IsRollup));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


