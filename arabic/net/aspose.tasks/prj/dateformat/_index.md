---
title: "Prj.DateFormat"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. تنسيق تاريخ عرض المشروع"
type: docs
weight: 210
url: /ar/net/aspose.tasks/prj/dateformat/
---
## Prj.DateFormat field

تنسيق تاريخ عرض المشروع.

```csharp
public static readonly Key<DateFormat, PrjKey> DateFormat;
```

## الأمثلة

يوضح كيفية قراءة/كتابة الخاصية Prj.DateFormat.

```csharp
var project = new Project();

project.Set(Prj.DateFormat, DateFormat.DateDd);

Console.WriteLine("Date Format: " + project.Get(Prj.DateFormat));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [DateFormat](../../dateformat/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


