---
title: "Rsc.RemainingOvertimeCost"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. El gasto de horas extra programado restante para un recurso"
type: docs
weight: 590
url: /es/net/aspose.tasks/rsc/remainingovertimecost/
---
## Rsc.RemainingOvertimeCost field

El gasto programado de horas extra restante para un recurso.

```csharp
public static readonly Key<decimal, RscKey> RemainingOvertimeCost;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.RemainingOvertimeCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeCost, 3);

Console.WriteLine("Remaining Overtime Cost: " + resource.Get(Rsc.RemainingOvertimeCost));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


