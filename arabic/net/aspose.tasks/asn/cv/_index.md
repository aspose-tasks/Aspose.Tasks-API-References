---
title: "Asn.CV"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. فرق تكلفة القيمة المكتسبة. CV هو الفرق بين BCWP (التكلفة المتوقعة للعمل المنجز) و ACWP (التكلفة الفعلية للعمل المنجز) للتعيينات"
type: docs
weight: 220
url: /ar/net/aspose.tasks/asn/cv/
---
## Asn.CV field

تباين تكلفة القيمة المكتسبة. CV هو الفرق بين BCWP (التكلفة المتوقعة للعمل المنفذ) و ACWP (التكلفة الفعلية للعمل المنفذ) للمهمة.

```csharp
public static readonly Key<double, AsnKey> CV;
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


