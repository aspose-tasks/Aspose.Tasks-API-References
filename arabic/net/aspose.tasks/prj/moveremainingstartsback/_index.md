---
title: "Prj.MoveRemainingStartsBack"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. يحدد ما إذا كان يجب إرجاع بداية الأجزاء المتبقية من المهام المجدولة للبدء بعد تاريخ الحالة ولكن التي بدأت مبكرًا إلى تاريخ الحالة"
type: docs
weight: 510
url: /ar/net/aspose.tasks/prj/moveremainingstartsback/
---
## Prj.MoveRemainingStartsBack field

يحدد ما إذا كان يجب إرجاع بداية الأجزاء المتبقية من المهام المجدولة للبدء بعد تاريخ الحالة ولكن التي بدأت مبكرًا إلى تاريخ الحالة.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsBack;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Prj.MoveRemainingStartsBack.

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsBack, true);

Console.WriteLine("Move Remaining Starts Back: " + project.Get(Prj.MoveRemainingStartsBack));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


