---
title: "Asn.SV"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. فرق جدول القيمة المكتسبة حتى تاريخ حالة المشروع. فرق الجدول الزمني SV هو الفرق بين BCWP و BCWS"
type: docs
weight: 540
url: /ar/net/aspose.tasks/asn/sv/
---
## Asn.SV field

انحراف جدول القيمة المكتسبة حتى تاريخ حالة المشروع. انحراف الجدول (SV) هو الفرق بين BCWP و BCWS.

```csharp
public static readonly Key<double, AsnKey> SV;
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


