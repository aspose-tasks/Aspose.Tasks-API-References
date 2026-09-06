---
title: "Prj.MoveRemainingStartsForward"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. يحدد ما إذا كان يجب نقل بداية الأجزاء المتبقية من المهام المجدولة للبدء لاحقًا إلى تاريخ الحالة"
type: docs
weight: 520
url: /ar/net/aspose.tasks/prj/moveremainingstartsforward/
---
## Prj.MoveRemainingStartsForward field

يحدد ما إذا كان يجب رفع بداية الأجزاء المتبقية من المهام المجدولة لتبدأ لاحقًا إلى تاريخ الحالة.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsForward;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Prj.MoveRemainingStartsForward.

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsForward, true);

Console.WriteLine("Move Remaining Starts Forward: " + project.Get(Prj.MoveRemainingStartsForward));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


