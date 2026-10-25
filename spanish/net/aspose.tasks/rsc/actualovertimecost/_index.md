---
title: "Rsc.ActualOvertimeCost"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. Costos incurridos por trabajo extra ya realizado en tareas por los recursos asignados"
type: docs
weight: 40
url: /es/net/aspose.tasks/rsc/actualovertimecost/
---
## Rsc.ActualOvertimeCost field

Costos incurridos por el trabajo de horas extra ya realizado en tareas por los recursos asignados.

```csharp
public static readonly Key<decimal, RscKey> ActualOvertimeCost;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.ActualOvertimeCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + resource.Get(Rsc.ActualOvertimeCost));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


