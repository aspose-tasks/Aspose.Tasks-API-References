---
title: "Rsc.RemainingCost"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. المصروف المجدول المتبقي الذي سيتكبد عند إكمال العمل المجدول المتبقي"
type: docs
weight: 580
url: /ar/net/aspose.tasks/rsc/remainingcost/
---
## Rsc.RemainingCost field

النفقات المجدولة المتبقية التي ستُتحمل عند إكمال العمل المجدول المتبقي.

```csharp
public static readonly Key<decimal, RscKey> RemainingCost;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.RemainingCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingCost, 2);

Console.WriteLine("Remaining Cost: " + resource.Get(Rsc.RemainingCost));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


