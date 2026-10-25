---
title: "Rsc.PercentWorkComplete"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. نسبة العمل المكتمل عبر جميع المهام"
type: docs
weight: 550
url: /ar/net/aspose.tasks/rsc/percentworkcomplete/
---
## Rsc.PercentWorkComplete field

نسبة العمل المكتمل عبر جميع المهام.

```csharp
public static readonly Key<int, RscKey> PercentWorkComplete;
```

## الأمثلة

يعرض كيفية قراءة نسبة إكمال العمل للمورد.

```csharp
var project = new Project(DataDir + "ResourcePercentWorkComplete.mpp");

// عرض نسبة إكمال العمل لجميع الموارد
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) != null)
    {
        Console.WriteLine(res.Get(Rsc.PercentWorkComplete));
    }
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


