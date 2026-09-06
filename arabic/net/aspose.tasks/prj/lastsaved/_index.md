---
title: "Prj.LastSaved"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. التاريخ الذي تم فيه حفظ المشروع آخر مرة. محفوظ بتنسيق UTC في ملفات mpp. نوع DateTime"
type: docs
weight: 440
url: /ar/net/aspose.tasks/prj/lastsaved/
---
## Prj.LastSaved field

التاريخ الذي تم فيه حفظ المشروع آخر مرة. محفوظ بصيغة UTC في ملفات mpp. نوع DateTime.

```csharp
public static readonly Key<DateTime, PrjKey> LastSaved;
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


