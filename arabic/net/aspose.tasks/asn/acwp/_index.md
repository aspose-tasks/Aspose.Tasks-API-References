---
title: "Asn.ACWP"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. التكلفة الفعلية للعمل المنفذ على تعيين حتى الآن"
type: docs
weight: 90
url: /ar/net/aspose.tasks/asn/acwp/
---
## Asn.ACWP field

التكلفة الفعلية للعمل المنفذ على مهمة حتى الآن.

```csharp
public static readonly Key<double, AsnKey> ACWP;
```

## الأمثلة

يوضح كيفية قراءة قيم تكلفة التعيين.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

// طباعة تكاليف تعيين الموارد
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

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


