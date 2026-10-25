---
title: "Prj.MoveCompletedEndsForward"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. يحدد ما إذا كان يجب نقل نهاية الأجزاء المكتملة من المهام المجدولة لتكون مكتملة قبل تاريخ الحالة ولكن بدأت لاحقًا إلى تاريخ الحالة"
type: docs
weight: 500
url: /ar/net/aspose.tasks/prj/movecompletedendsforward/
---
## Prj.MoveCompletedEndsForward field

يحدد ما إذا كان يجب رفع نهاية الأجزاء المكتملة من المهام المجدولة لتكون قد اكتملت قبل تاريخ الحالة ولكن بدأت لاحقًا إلى تاريخ الحالة.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsForward;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Prj.MoveCompletedEndsForward.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsForward, true);

Console.WriteLine("Move Completed Ends Forward: " + project.Get(Prj.MoveCompletedEndsForward));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


