---
title: "Rsc.CostVariance"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. La diferencia entre el costo de referencia y el costo total de un recurso"
type: docs
weight: 250
url: /es/net/aspose.tasks/rsc/costvariance/
---
## Rsc.CostVariance field

La diferencia entre el costo de referencia y el costo total para un recurso.

```csharp
public static readonly Key<double, RscKey> CostVariance;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.CostVariance.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostVariance, 10);

Console.WriteLine("Cost Variance: " + resource.Get(Rsc.CostVariance));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


