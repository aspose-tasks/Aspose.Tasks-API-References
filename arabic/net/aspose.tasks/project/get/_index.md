---
title: "Project.Get"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Project. تُرجع القيمة التي تم ربط الخاصية بها في هذا الحاوية"
type: docs
weight: 1080
url: /ar/net/aspose.tasks/project/get/
---
## Project.Get&lt;T&gt; method

يعيد القيمة التي تم ربط الخاصية بها في هذه الحاوية.

```csharp
public T Get<T>(Key<T, PrjKey> key)
```

| معامل | الوصف |
| --- | --- |
| T | نوع القيمة المرتبطة. |
| key | مفتاح الخاصية المحددة. [`Prj`](../../prj/) للحصول على مفتاح الخاصية. |

### قيمة الإرجاع

القيمة التي تم تعيين الخاصية إليها في هذا الحاوية.

## الأمثلة

يوضح كيفية التحقق من نسخة المشروع.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// عرض نسخة المشروع
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


