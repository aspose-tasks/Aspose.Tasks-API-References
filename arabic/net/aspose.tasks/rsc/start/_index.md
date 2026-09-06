---
title: "Rsc.Start"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. التاريخ الذي يُجدول فيه المورد المعين بدء العمل على مهمة"
type: docs
weight: 640
url: /ar/net/aspose.tasks/rsc/start/
---
## Rsc.Start field

التاريخ الذي يُجدول فيه المورد المعين لبدء العمل على مهمة.

```csharp
public static readonly Key<DateTime, RscKey> Start;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Rsc.Start.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Start, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Start: " + resource.Get(Rsc.Start));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


