---
title: "Rsc.AccrueAt"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. يحدد كيف ومتى يتم تحميل أو تراكم تكاليف المورد القياسية والعمل الإضافي إلى تكلفة المهمة"
type: docs
weight: 10
url: /ar/net/aspose.tasks/rsc/accrueat/
---
## Rsc.AccrueAt field

يحدد كيف ومتى يتم تحميل أو تراكم تكاليف المورد القياسية والزيادة على تكلفة المهمة.

```csharp
public static readonly Key<CostAccrualType, RscKey> AccrueAt;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.AccrueAt.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AccrueAt, CostAccrualType.End);

Console.WriteLine("Accrue At: " + resource.Get(Rsc.AccrueAt));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


