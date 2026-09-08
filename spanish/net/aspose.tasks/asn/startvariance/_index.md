---
title: "Asn.StartVariance"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. La variación de la fecha de inicio de una asignación respecto a la fecha de inicio de referencia"
type: docs
weight: 510
url: /es/net/aspose.tasks/asn/startvariance/
---
## Asn.StartVariance field

La variación de la fecha de inicio de una asignación respecto a la fecha de inicio de referencia.

```csharp
public static readonly Key<Duration, AsnKey> StartVariance;
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
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


