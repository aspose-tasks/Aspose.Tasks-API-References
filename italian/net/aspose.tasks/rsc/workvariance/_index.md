---
title: "Rsc.WorkVariance"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. La differenza tra il lavoro di base di una risorsa e il lavoro attualmente programmato"
type: docs
weight: 710
url: /it/net/aspose.tasks/rsc/workvariance/
---
## Rsc.WorkVariance field

La differenza tra il lavoro di baseline di una risorsa e il lavoro attualmente programmato.

```csharp
public static readonly Key<double, RscKey> WorkVariance;
```

## Esempi

Mostra come leggere la varianza del lavoro della risorsa.

```csharp
var project = new Project(DataDir + "WorkVariance.mpp");

foreach (var assignment in project.ResourceAssignments)
{
    var resource = assignment.Get(Asn.Resource);

    var workVariance = resource.Get(Rsc.WorkVariance);

    Console.WriteLine(workVariance);
}
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


