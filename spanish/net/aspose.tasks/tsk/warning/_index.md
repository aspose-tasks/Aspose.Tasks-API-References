---
title: "Tsk.Warning"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Representa la bandera que indica que la tarea tiene discrepancias de programación"
type: docs
weight: 1120
url: /es/net/aspose.tasks/tsk/warning/
---
## Tsk.Warning field

Representa la bandera que indica que la tarea tiene discrepancias de programación.

```csharp
public static readonly Key<bool, TaskKey> Warning;
```

## Ejemplos

Muestra cómo leer una advertencia de tarea.

```csharp
var project = new Project(DataDir + "schedule-conflict.mpp");
var task = project.RootTask.Children.GetById(1);
Console.WriteLine(task.Get(Tsk.Warning));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


