---
title: "Asn.PercentWorkComplete"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Asn. La cantidad de trabajo completado en una asignación"
type: docs
weight: 400
url: /es/net/aspose.tasks/asn/percentworkcomplete/
---
## Asn.PercentWorkComplete field

La cantidad de trabajo completado en una asignación.

```csharp
public static readonly Key<int, AsnKey> PercentWorkComplete;
```

## Ejemplos

Muestra cómo leer el porcentaje de trabajo completado de una asignación.

```csharp
var project = new Project(DataDir + "ResourceAssignmentPercentWorkComplete.mpp");

// Imprimir porcentaje de finalización de la asignación
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.PercentWorkComplete).ToString());
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


