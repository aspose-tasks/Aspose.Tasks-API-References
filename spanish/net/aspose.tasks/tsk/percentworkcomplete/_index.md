---
title: "Tsk.PercentWorkComplete"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. El estado actual de una tarea expresado como el porcentaje del trabajo que se ha completado."
type: docs
weight: 890
url: /es/net/aspose.tasks/tsk/percentworkcomplete/
---
## Tsk.PercentWorkComplete field

El estado actual de una tarea expresado como el porcentaje del trabajo que se ha completado.

```csharp
public static readonly Key<int, TaskKey> PercentWorkComplete;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.PercentWorkComplete.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PercentWorkComplete, 10);

Console.WriteLine("Percent Work Complete: " + task.Get(Tsk.PercentWorkComplete));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


