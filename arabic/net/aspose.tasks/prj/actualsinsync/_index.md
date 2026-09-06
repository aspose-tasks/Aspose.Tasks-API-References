---
title: "Prj.ActualsInSync"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. يحدد ما إذا كان جميع الأعمال الفعلية قد تمت مزامنتها مع المشروع"
type: docs
weight: 10
url: /ar/net/aspose.tasks/prj/actualsinsync/
---
## Prj.ActualsInSync field

يحدد ما إذا كان جميع الأعمال الفعلية قد تم مزامنتها مع المشروع.

```csharp
public static readonly Key<NullableBool, PrjKey> ActualsInSync;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Prj.ActualsInSync.

```csharp
var project = new Project();

project.Set(Prj.ActualsInSync, true);

Console.WriteLine("Actuals In Sync: " + project.Get(Prj.ActualsInSync));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


