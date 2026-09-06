---
title: "Rsc.ActualOvertimeCost"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. التكاليف المتكبدة للعمل الإضافي الذي تم إنجازه بالفعل على المهام بواسطة الموارد المعينة"
type: docs
weight: 40
url: /ar/net/aspose.tasks/rsc/actualovertimecost/
---
## Rsc.ActualOvertimeCost field

التكاليف المتكبدة للعمل الإضافي الذي تم إنجازه بالفعل على المهام بواسطة الموارد المعينة.

```csharp
public static readonly Key<decimal, RscKey> ActualOvertimeCost;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.ActualOvertimeCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + resource.Get(Rsc.ActualOvertimeCost));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


