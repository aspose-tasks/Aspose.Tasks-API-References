---
title: "Prj.StatusDate"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. تاريخ الحالة لعرض التقدم أو لحساب إجماليات القيمة المكتسبة. تاريخ الحالة هو نفسه تاريخ اليوم الحالي ما لم يتم تحديد تاريخ حالة مختلف"
type: docs
weight: 690
url: /ar/net/aspose.tasks/prj/statusdate/
---
## Prj.StatusDate field

تاريخ الحالة لعرض التقدم أو لحساب إجماليات القيمة المكتسبة. تاريخ الحالة هو نفسه التاريخ الحالي (تاريخ اليوم) ما لم يتم تحديد تاريخ حالة مختلف.

```csharp
public static readonly Key<DateTime, PrjKey> StatusDate;
```

## الأمثلة

يوضح كيفية قراءة/كتابة الخاصية Prj.StatusDate.

```csharp
var project = new Project();

project.Set(Prj.StatusDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Status Date: " + project.Get(Prj.StatusDate));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


