---
title: "Prj.TimescaleStart"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. التاريخ الذي يبدأ فيه المقياس الزمني في العرض"
type: docs
weight: 740
url: /ar/net/aspose.tasks/prj/timescalestart/
---
## Prj.TimescaleStart field

التاريخ الذي يبدأ فيه مقياس الوقت في العرض.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleStart;
```

## الأمثلة

يعرض كيفية تعيين تاريخ بدء المقياس الزمني لضبط التاريخ الذي يجب أن يبدأ فيه العرض.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.TimescaleStart, new DateTime(2012, 4, 30));

Console.WriteLine("Timescale Start: " + project.Get(Prj.TimescaleStart));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


