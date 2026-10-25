---
title: "Prj.LastPrinted"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. وقت الطباعة الأخير للمشروع. محفوظ بتنسيق UTC في ملفات mpp. نوع DateTime"
type: docs
weight: 430
url: /ar/net/aspose.tasks/prj/lastprinted/
---
## Prj.LastPrinted field

وقت الطباعة الأخير للمشروع. محفوظ بصيغة UTC في ملفات mpp. نوع DateTime.

```csharp
public static readonly Key<DateTime, PrjKey> LastPrinted;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Prj.LastPrinted.

```csharp
var project = new Project();

project.Set(Prj.LastPrinted, new DateTime(2020, 4, 10, 13, 0, 0));

Console.WriteLine("Last Printed: " + project.Get(Prj.LastPrinted));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


