---
title: "Tsk.PhysicalPercentComplete"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Valor de porcentaje completado que puede usarse como alternativa para calcular el costo presupuestado del trabajo realizado (BCWP)"
type: docs
weight: 900
url: /es/net/aspose.tasks/tsk/physicalpercentcomplete/
---
## Tsk.PhysicalPercentComplete field

Valor de porcentaje completado que puede usarse como alternativa para calcular el costo presupuestado del trabajo realizado (BCWP).

```csharp
public static readonly Key<int, TaskKey> PhysicalPercentComplete;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.PhysicalPercentComplete.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PhysicalPercentComplete, 10);

Console.WriteLine("Physical Percent Complete: " + task.Get(Tsk.PhysicalPercentComplete));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


