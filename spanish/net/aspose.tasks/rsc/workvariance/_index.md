---
title: "Rsc.WorkVariance"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Rsc. La diferencia entre el trabajo base de un recurso y el trabajo programado actualmente"
type: docs
weight: 710
url: /es/net/aspose.tasks/rsc/workvariance/
---
## Rsc.WorkVariance field

La diferencia entre el trabajo de referencia de un recurso y el trabajo actualmente programado.

```csharp
public static readonly Key<double, RscKey> WorkVariance;
```

## Ejemplos

Muestra cómo leer la variación de trabajo del recurso.

```csharp
var project = new Project(DataDir + "WorkVariance.mpp");

foreach (var assignment in project.ResourceAssignments)
{
    var resource = assignment.Get(Asn.Resource);

    var workVariance = resource.Get(Rsc.WorkVariance);

    Console.WriteLine(workVariance);
}
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


