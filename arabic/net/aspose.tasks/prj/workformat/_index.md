---
title: "Prj.WorkFormat"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. الصيغة المستخدمة لعرض مدة المهمة"
type: docs
weight: 790
url: /ar/net/aspose.tasks/prj/workformat/
---
## Prj.WorkFormat field

الصيغة المستخدمة لعرض مدة المهمة.

```csharp
public static readonly Key<TimeUnitType, PrjKey> WorkFormat;
```

## الأمثلة

يوضح كيفية الحصول على مدة باستخدام صيغة العمل الافتراضية.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// إنشاء قيمة عمل باستخدام تنسيق العمل الافتراضي للمشروع
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


