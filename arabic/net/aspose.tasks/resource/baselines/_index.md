---
title: "Resource.Baselines"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Resource. تحصل على مثيل BaselineCollection لهذا الكائن. قيم الخط الأساسي لمورد"
type: docs
weight: 160
url: /ar/net/aspose.tasks/resource/baselines/
---
## Resource.Baselines property

يحصل على نسخة من BaselineCollection لهذا الكائن. القيم الأساسية للمورد.

```csharp
public BaselineCollection Baselines { get; }
```

## الأمثلة

يوضح كيفية قراءة الخطوط الأساسية للمورد.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

foreach (var resource in project.Resources)
{
    foreach (var baseline in resource.Baselines)
    {
        Console.WriteLine("BaselineNumber: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
    }
}
```

### انظر أيضًا

* class [BaselineCollection](../../baselinecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


