---
title: "Rsc.ActualCost"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. التكاليف المتكبدة للعمل الذي أُنجز بالفعل من قبل الموارد على مهامهم بالإضافة إلى أي تكاليف مسجلة أخرى مرتبطة بالمهمة"
type: docs
weight: 30
url: /ar/net/aspose.tasks/rsc/actualcost/
---
## Rsc.ActualCost field

التكاليف المتكبدة للعمل الذي قام به الموارد بالفعل على مهامهم، إلى جانب أي تكاليف مسجلة أخرى مرتبطة بالمهمة.

```csharp
public static readonly Key<decimal, RscKey> ActualCost;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.ActualCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualCost, 10m);

Console.WriteLine("Actual Cost: " + resource.Get(Rsc.ActualCost));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


