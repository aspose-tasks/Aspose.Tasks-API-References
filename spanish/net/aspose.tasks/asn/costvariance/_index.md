---
title: "Asn.CostVariance"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. La diferencia entre el costo de referencia y el costo total de una asignación"
type: docs
weight: 200
url: /es/net/aspose.tasks/asn/costvariance/
---
## Asn.CostVariance field

La diferencia entre el costo de referencia y el costo total de una asignación.

```csharp
public static readonly Key<double, AsnKey> CostVariance;
```

## Ejemplos

Muestra cómo leer las variaciones de la asignación.

```csharp
var project = new Project(DataDir + "ResourceAssignmentVariance.mpp");

// Imprimir variaciones de la asignación
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.WorkVariance));
    Console.WriteLine(ra.Get(Asn.CostVariance));
    Console.WriteLine(ra.Get(Asn.StartVariance));
    Console.WriteLine(ra.Get(Asn.FinishVariance));
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


