---
title: "Prj.StartDate"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. تاريخ بدء المشروع"
type: docs
weight: 680
url: /ar/net/aspose.tasks/prj/startdate/
---
## Prj.StartDate field

تاريخ بدء المشروع.

```csharp
public static readonly Key<DateTime, PrjKey> StartDate;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Prj.StartDate.

```csharp
var project = new Project();

project.Set(Prj.StartDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Start Date: " + project.Get(Prj.StartDate));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


