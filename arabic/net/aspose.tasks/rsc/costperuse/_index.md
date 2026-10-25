---
title: "Rsc.CostPerUse"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. التكلفة التي تتراكم في كل مرة يتم فيها استخدام المورد"
type: docs
weight: 240
url: /ar/net/aspose.tasks/rsc/costperuse/
---
## Rsc.CostPerUse field

التكلفة التي تتراكم في كل مرة يتم فيها استخدام المورد.

```csharp
public static readonly Key<decimal, RscKey> CostPerUse;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Rsc.CostPerUse.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostPerUse, 9);

Console.WriteLine("Cost Per Use: " + resource.Get(Rsc.CostPerUse));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


