---
title: "Rsc.CostCenter"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. يحدد مركز التكلفة الذي يجب تحميل التكاليف المتراكمة للمورد إليه"
type: docs
weight: 230
url: /ar/net/aspose.tasks/rsc/costcenter/
---
## Rsc.CostCenter field

يشير إلى مركز التكلفة الذي يجب تحميل التكاليف المتراكمة للمورد إليه.

```csharp
public static readonly Key<string, RscKey> CostCenter;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Rsc.CostCenter.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostCenter, "Center");

Console.WriteLine("Cost Center: " + resource.Get(Rsc.CostCenter));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


