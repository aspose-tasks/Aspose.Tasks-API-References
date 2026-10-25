---
title: "Prj.MultipleCriticalPaths"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. يحدد ما إذا تم حساب مسارات حرجة متعددة."
type: docs
weight: 530
url: /ar/net/aspose.tasks/prj/multiplecriticalpaths/
---
## Prj.MultipleCriticalPaths field

يحدد ما إذا كان يتم حساب مسارات حرجة متعددة.

```csharp
public static readonly Key<NullableBool, PrjKey> MultipleCriticalPaths;
```

## الأمثلة

يوضح كيفية قراءة/كتابة الخاصية Prj.MultipleCriticalPaths.

```csharp
var project = new Project();

project.Set(Prj.MultipleCriticalPaths, true);

Console.WriteLine("Multiple Critical Paths: " + project.Get(Prj.MultipleCriticalPaths));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


