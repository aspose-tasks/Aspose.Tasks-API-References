---
title: "Asn.PercentWorkComplete"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. مقدار العمل المكتمل على تعيين"
type: docs
weight: 400
url: /ar/net/aspose.tasks/asn/percentworkcomplete/
---
## Asn.PercentWorkComplete field

كمية العمل المنجز في مهمة.

```csharp
public static readonly Key<int, AsnKey> PercentWorkComplete;
```

## الأمثلة

يعرض كيفية قراءة نسبة إكمال العمل لتعيين.

```csharp
var project = new Project(DataDir + "ResourceAssignmentPercentWorkComplete.mpp");

// طباعة نسبة إكمال التعيين
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.PercentWorkComplete).ToString());
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


