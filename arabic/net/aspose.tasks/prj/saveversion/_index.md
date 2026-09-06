---
title: "Prj.SaveVersion"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. إصدار Microsoft Office Project الذي تم حفظ ملف المشروع منه"
type: docs
weight: 620
url: /ar/net/aspose.tasks/prj/saveversion/
---
## Prj.SaveVersion field

إصدار Microsoft Office Project الذي تم حفظ ملف المشروع منه.

```csharp
public static readonly Key<int, PrjKey> SaveVersion;
```

## الأمثلة

يعرض كيفية التحقق من نسخة حفظ المشروع وتاريخ الحفظ.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// عرض نسخة المشروع
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


