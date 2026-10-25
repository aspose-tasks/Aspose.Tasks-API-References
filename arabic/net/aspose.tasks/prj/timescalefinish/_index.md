---
title: "Prj.TimescaleFinish"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. التاريخ الذي ينتهي فيه المقياس الزمني في العرض"
type: docs
weight: 730
url: /ar/net/aspose.tasks/prj/timescalefinish/
---
## Prj.TimescaleFinish field

التاريخ الذي ينتهي فيه مقياس الوقت في العرض.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleFinish;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Prj.TimescaleFinish.

```csharp
var project = new Project();

project.Set(Prj.TimescaleFinish, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Timescale Finish: " + project.Get(Prj.TimescaleFinish));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


