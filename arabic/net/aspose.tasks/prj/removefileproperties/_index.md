---
title: "Prj.RemoveFileProperties"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. يحدد ما إذا كان سيتم إزالة جميع خصائص الملف عند الحفظ"
type: docs
weight: 600
url: /ar/net/aspose.tasks/prj/removefileproperties/
---
## Prj.RemoveFileProperties field

يحدد ما إذا سيتم إزالة جميع خصائص الملف عند الحفظ.

```csharp
public static readonly Key<NullableBool, PrjKey> RemoveFileProperties;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Prj.RemoveFileProperties.

```csharp
var project = new Project();

project.Set(Prj.RemoveFileProperties, true);

Console.WriteLine("Remove File Properties: " + project.Get(Prj.RemoveFileProperties));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


