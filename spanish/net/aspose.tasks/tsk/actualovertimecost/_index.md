---
title: "Tsk.ActualOvertimeCost"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Costos incurridos por trabajo extra ya realizado en tareas por los recursos asignados"
type: docs
weight: 50
url: /es/net/aspose.tasks/tsk/actualovertimecost/
---
## Tsk.ActualOvertimeCost field

Costos incurridos por el trabajo de horas extra ya realizado en tareas por los recursos asignados.

```csharp
public static readonly Key<decimal, TaskKey> ActualOvertimeCost;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.ActualOvertimeCost.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + task.Get(Tsk.ActualOvertimeCost));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


