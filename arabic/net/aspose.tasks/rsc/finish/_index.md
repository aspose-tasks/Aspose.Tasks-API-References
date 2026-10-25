---
title: "Rsc.Finish"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. التاريخ الذي يُجدول فيه المورد لإكمال العمل على جميع المهام المعينة"
type: docs
weight: 290
url: /ar/net/aspose.tasks/rsc/finish/
---
## Rsc.Finish field

التاريخ الذي من المقرر فيه أن يكمل المورد العمل على جميع المهام المعينة.

```csharp
public static readonly Key<DateTime, RscKey> Finish;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.Finish.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Finish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Finish: " + resource.Get(Rsc.Finish));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


