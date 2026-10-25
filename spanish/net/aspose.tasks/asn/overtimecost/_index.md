---
title: "Asn.OvertimeCost"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. La suma del costo real y restante de horas extra de una asignación"
type: docs
weight: 370
url: /es/net/aspose.tasks/asn/overtimecost/
---
## Asn.OvertimeCost field

La suma del costo real y del costo restante de horas extra de una asignación.

```csharp
public static readonly Key<decimal, AsnKey> OvertimeCost;
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


