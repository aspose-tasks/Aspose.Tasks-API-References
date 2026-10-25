---
title: "Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. يحدد ما إذا كان يجب الحفاظ على المهام اليدوية في أقرب وقت عمل عند تحويلها إلى مجدولة تلقائيًا"
type: docs
weight: 400
url: /ar/net/aspose.tasks/prj/keeptaskonnearestworkingtimewhenmadeautoscheduled/
---
## Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled field

يحدد ما إذا كان يجب الحفاظ على المهام اليدوية في أقرب وقت عمل عند تحويلها إلى جدول تلقائي.

```csharp
public static readonly Key<NullableBool, PrjKey> KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled.

```csharp
var project = new Project();

project.Set(Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled, true);

Console.WriteLine("Keep Task On Nearest Working Time When Made Auto Scheduled: " + project.Get(Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


