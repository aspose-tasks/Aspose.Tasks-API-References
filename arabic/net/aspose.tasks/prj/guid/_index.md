---
title: "Prj.Guid"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. المعرف الفريد للمشروع"
type: docs
weight: 360
url: /ar/net/aspose.tasks/prj/guid/
---
## Prj.Guid field

معرف GUID للمشروع.

```csharp
public static readonly Key<Guid, PrjKey> Guid;
```

## الأمثلة

يُظهر كيفية قراءة/كتابة خاصية Prj.Guid.

```csharp
var project = new Project();

project.Set(Prj.Guid, new Guid("efcc0d63-d8e0-4a34-9f3e-9f973f50238a"));

Console.WriteLine("Guid: " + project.Get(Prj.Guid));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


