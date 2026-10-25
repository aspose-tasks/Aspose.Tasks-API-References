---
title: "Asn.WorkVariance"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. La diferencia entre el trabajo de referencia de una tarea y el trabajo actualmente programado"
type: docs
weight: 620
url: /es/net/aspose.tasks/asn/workvariance/
---
## Asn.WorkVariance field

La diferencia entre el trabajo de línea base de una tarea y el trabajo programado actualmente.

```csharp
public static readonly Key<Duration, AsnKey> WorkVariance;
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


