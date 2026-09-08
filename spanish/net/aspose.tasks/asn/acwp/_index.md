---
title: "Asn.ACWP"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. El costo real del trabajo realizado en una asignación hasta la fecha"
type: docs
weight: 90
url: /es/net/aspose.tasks/asn/acwp/
---
## Asn.ACWP field

El costo real de un trabajo realizado en una asignación hasta la fecha.

```csharp
public static readonly Key<double, AsnKey> ACWP;
```

## Ejemplos

Muestra cómo leer los valores de costo de la asignación.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

// Imprimir costos de asignación de recursos
foreach (var assignment in project.ResourceAssignments)
{
    Console.WriteLine(assignment.Get(Asn.Cost));
    Console.WriteLine(assignment.Get(Asn.ACWP));

    // CV = BCWP - ACWP
    Console.WriteLine(assignment.Get(Asn.CV));

    Console.WriteLine(assignment.Get(Asn.BCWP));
    Console.WriteLine(assignment.Get(Asn.BCWS));

    // SV = BCWP - BCWS
    Console.WriteLine(assignment.Get(Asn.SV));
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


