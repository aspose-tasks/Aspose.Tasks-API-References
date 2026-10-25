---
title: "Rsc.RemainingCost"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Rsc campo. El gasto programado restante que se incurrirá al completar el trabajo programado restante"
type: docs
weight: 580
url: /es/net/aspose.tasks/rsc/remainingcost/
---
## Rsc.RemainingCost field

El gasto programado restante que se incurrirá al completar el trabajo programado restante.

```csharp
public static readonly Key<decimal, RscKey> RemainingCost;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Rsc.RemainingCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingCost, 2);

Console.WriteLine("Remaining Cost: " + resource.Get(Rsc.RemainingCost));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


