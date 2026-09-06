---
title: "Rsc.WorkVariance"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. الفرق بين العمل الأساسي لمورد والعمل المجدول حالياً"
type: docs
weight: 710
url: /ar/net/aspose.tasks/rsc/workvariance/
---
## Rsc.WorkVariance field

الفرق بين العمل الأساسي للمورد والعمل المجدول حاليًا.

```csharp
public static readonly Key<double, RscKey> WorkVariance;
```

## الأمثلة

يظهر كيفية قراءة تباين عمل المورد.

```csharp
var project = new Project(DataDir + "WorkVariance.mpp");

foreach (var assignment in project.ResourceAssignments)
{
    var resource = assignment.Get(Asn.Resource);

    var workVariance = resource.Get(Rsc.WorkVariance);

    Console.WriteLine(workVariance);
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


