---
title: "Asn.SV"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. La variación del cronograma del valor ganado hasta la fecha de estado del proyecto. La variación del cronograma SV es la diferencia entre BCWP y BCWS"
type: docs
weight: 540
url: /es/net/aspose.tasks/asn/sv/
---
## Asn.SV field

La variación del cronograma del valor ganado, hasta la fecha de estado del proyecto. La variación del cronograma (SV) es la diferencia entre el BCWP y el BCWS.

```csharp
public static readonly Key<double, AsnKey> SV;
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


