---
title: "Prj.CustomDateFormat"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. تنسيق التاريخ المخصص لعرض المشروع. يُستخدم لتنسيق التواريخ عندما تكون الخاصية DateFormat مضبوطة على Custom"
type: docs
weight: 200
url: /ar/net/aspose.tasks/prj/customdateformat/
---
## Prj.CustomDateFormat field

تنسيق التاريخ المخصص لعرض المشروع. يُستخدم لتنسيق التواريخ عندما تكون الخاصية [`DateFormat`](../dateformat/) مضبوطة على Custom.

```csharp
public static readonly Key<string, PrjKey> CustomDateFormat;
```

## الأمثلة

يوضح كيفية قراءة/كتابة الخاصية Prj.CustomDateFormat.

```csharp
var project = new Project();

project.Set(Prj.CustomDateFormat, "dd MMMM yyyy H:mm");

Console.WriteLine("Custom Date Format: " + project.Get(Prj.CustomDateFormat));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


