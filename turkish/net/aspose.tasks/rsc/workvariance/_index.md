---
title: "Rsc.WorkVariance"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynağın temel iş miktarı ile şu anda planlanan iş arasındaki fark."
type: docs
weight: 710
url: /tr/net/aspose.tasks/rsc/workvariance/
---
## Rsc.WorkVariance field

Bir kaynağın temel iş ile şu anda planlanan iş arasındaki fark.

```csharp
public static readonly Key<double, RscKey> WorkVariance;
```

## Örnekler

Kaynak iş varyansını nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "WorkVariance.mpp");

foreach (var assignment in project.ResourceAssignments)
{
    var resource = assignment.Get(Asn.Resource);

    var workVariance = resource.Get(Rsc.WorkVariance);

    Console.WriteLine(workVariance);
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


