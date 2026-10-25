---
title: "Asn.RemainingCost"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. El costo proyectado restante para completar una asignación"
type: docs
weight: 430
url: /es/net/aspose.tasks/asn/remainingcost/
---
## Asn.RemainingCost field

El costo proyectado restante de completar una asignación.

```csharp
public static readonly Key<decimal, AsnKey> RemainingCost;
```

## Ejemplos

Muestra cómo leer las horas extra/trabajos/costes restantes de una asignación.

```csharp
var project = new Project(DataDir + "ResourceAssignmentOvertimes.mpp");

// Imprimir horas extra de la asignación
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.OvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.OvertimeCost));
    Console.WriteLine(ra.Get(Asn.RemainingWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingCost));
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeCost));
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


