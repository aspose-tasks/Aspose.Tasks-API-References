---
title: "Rsc.RemainingOvertimeCost"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. المصروف المتبقي للوقت الإضافي المجدول لمورد"
type: docs
weight: 590
url: /ar/net/aspose.tasks/rsc/remainingovertimecost/
---
## Rsc.RemainingOvertimeCost field

نفقات العمل الإضافي المجدولة المتبقية للمورد.

```csharp
public static readonly Key<decimal, RscKey> RemainingOvertimeCost;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Rsc.RemainingOvertimeCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeCost, 3);

Console.WriteLine("Remaining Overtime Cost: " + resource.Get(Rsc.RemainingOvertimeCost));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


