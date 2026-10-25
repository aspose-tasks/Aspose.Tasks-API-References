---
title: "Rsc.ActualCost"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. Costos incurridos por el trabajo ya realizado por los recursos en sus tareas, junto con cualquier otro costo registrado asociado a la tarea"
type: docs
weight: 30
url: /es/net/aspose.tasks/rsc/actualcost/
---
## Rsc.ActualCost field

Costos incurridos por el trabajo ya realizado por los recursos en sus tareas, junto con cualquier otro costo registrado asociado a la tarea.

```csharp
public static readonly Key<decimal, RscKey> ActualCost;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.ActualCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualCost, 10m);

Console.WriteLine("Actual Cost: " + resource.Get(Rsc.ActualCost));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


