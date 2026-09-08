---
title: "Asn.BCWS"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. El costo presupuestado de un trabajo en la asignación"
type: docs
weight: 130
url: /es/net/aspose.tasks/asn/bcws/
---
## Asn.BCWS field

El costo presupuestado del trabajo en la asignación.

```csharp
public static readonly Key<double, AsnKey> BCWS;
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


