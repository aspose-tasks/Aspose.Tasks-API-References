---
title: "Rsc.CostPerUse"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. El costo que se genera cada vez que se utiliza un recurso"
type: docs
weight: 240
url: /es/net/aspose.tasks/rsc/costperuse/
---
## Rsc.CostPerUse field

El costo que se acumula cada vez que se utiliza un recurso.

```csharp
public static readonly Key<decimal, RscKey> CostPerUse;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.CostPerUse.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostPerUse, 9);

Console.WriteLine("Cost Per Use: " + resource.Get(Rsc.CostPerUse));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


