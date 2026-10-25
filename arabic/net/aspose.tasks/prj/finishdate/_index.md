---
title: "Prj.FinishDate"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. تاريخ الانتهاء لمشروع"
type: docs
weight: 330
url: /ar/net/aspose.tasks/prj/finishdate/
---
## Prj.FinishDate field

تاريخ الانتهاء للمشروع.

```csharp
public static readonly Key<DateTime, PrjKey> FinishDate;
```

## الأمثلة

يوضح كيفية إعادة جدولة المشروع من تاريخ الانتهاء بدلاً من تاريخ البدء.

```csharp
var project = new Project();
project.Set(Prj.ScheduleFromStart, false);
project.Set(Prj.FinishDate, new DateTime(2020, 1, 1));

// الآن يتم حساب جميع تواريخ المهام (Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish). للحصول على المسار الحرج نحتاج إلى حساب الفواصل (يمكن استدعاؤها في خيط منفصل، ولكن فقط بعد حساب جميع تواريخ البدء/الانتهاء المبكرة والمتأخرة).
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


