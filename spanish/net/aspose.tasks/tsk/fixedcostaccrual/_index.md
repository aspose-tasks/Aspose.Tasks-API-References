---
title: "Tsk.FixedCostAccrual"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Tsk. Determina las opciones de cómo y cuándo se deben cargar o acumular los costos fijos al costo de una tarea"
type: docs
weight: 440
url: /es/net/aspose.tasks/tsk/fixedcostaccrual/
---
## Tsk.FixedCostAccrual field

Determina las opciones de cómo y cuándo se deben cargar, o acumular, los costos fijos al costo de una tarea.

```csharp
public static readonly Key<CostAccrualType, TaskKey> FixedCostAccrual;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Tsk.FixedCostAccrual.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FixedCostAccrual, CostAccrualType.Prorated);

Console.WriteLine("Fixed Cost Accrual: " + task.Get(Tsk.FixedCostAccrual));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


