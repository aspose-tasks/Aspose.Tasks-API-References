---
title: "Rsc.CostVariance"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. الفرق بين التكلفة الأساسية والتكلفة الإجمالية لمورد"
type: docs
weight: 250
url: /ar/net/aspose.tasks/rsc/costvariance/
---
## Rsc.CostVariance field

الفرق بين تكلفة الخط الأساسي والتكلفة الإجمالية لمورد.

```csharp
public static readonly Key<double, RscKey> CostVariance;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Rsc.CostVariance.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostVariance, 10);

Console.WriteLine("Cost Variance: " + resource.Get(Rsc.CostVariance));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


