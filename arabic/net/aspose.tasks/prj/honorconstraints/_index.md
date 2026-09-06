---
title: "Prj.HonorConstraints"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. يحدد ما إذا كانت المهام تحترم تواريخ القيود الخاصة بها"
type: docs
weight: 370
url: /ar/net/aspose.tasks/prj/honorconstraints/
---
## Prj.HonorConstraints field

يحدد ما إذا كانت المهام تحترم تواريخ القيود الخاصة بها.

```csharp
public static readonly Key<NullableBool, PrjKey> HonorConstraints;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Prj.HonorConstraints.

```csharp
var project = new Project();

project.Set(Prj.HonorConstraints, true);

Console.WriteLine("Honor Constraints: " + project.Get(Prj.HonorConstraints));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


