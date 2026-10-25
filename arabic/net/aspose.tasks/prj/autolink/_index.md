---
title: "Prj.Autolink"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. يحدد ما إذا كانت المهام المُدخلة أو المنقولة مرتبطة تلقائيًا"
type: docs
weight: 70
url: /ar/net/aspose.tasks/prj/autolink/
---
## Prj.Autolink field

يحدد ما إذا كانت المهام المدخلة أو المنقولة مرتبطة تلقائيًا.

```csharp
public static readonly Key<NullableBool, PrjKey> Autolink;
```

## الأمثلة

يُظهر كيفية قراءة/كتابة خاصية Prj.Autolink.

```csharp
var project = new Project();

project.Set(Prj.Autolink, true);

Console.WriteLine("Autolink: " + project.Get(Prj.Autolink));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


