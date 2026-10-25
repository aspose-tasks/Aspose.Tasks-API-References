---
title: "Prj.MoveCompletedEndsBack"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. يحدد ما إذا كان يجب إرجاع نهاية الأجزاء المكتملة من المهام المجدولة للبدء بعد تاريخ الحالة ولكن التي بدأت مبكرًا إلى تاريخ الحالة"
type: docs
weight: 490
url: /ar/net/aspose.tasks/prj/movecompletedendsback/
---
## Prj.MoveCompletedEndsBack field

يحدد ما إذا كان يجب إرجاع نهاية الأجزاء المكتملة من المهام المجدولة للبدء بعد تاريخ الحالة ولكن التي بدأت مبكرًا إلى تاريخ الحالة.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsBack;
```

## الأمثلة

يُظهر كيفية قراءة/كتابة خاصية Prj.MoveCompletedEndsBack.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsBack, true);

Console.WriteLine("Move Completed Ends Back: " + project.Get(Prj.MoveCompletedEndsBack));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


