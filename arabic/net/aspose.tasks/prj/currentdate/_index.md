---
title: "Prj.CurrentDate"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. تاريخ النظام"
type: docs
weight: 190
url: /ar/net/aspose.tasks/prj/currentdate/
---
## Prj.CurrentDate field

تاريخ النظام.

```csharp
public static readonly Key<DateTime, PrjKey> CurrentDate;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Prj.CurrentDate.

```csharp
var project = new Project();

project.Set(Prj.CurrentDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Current Date: " + project.Get(Prj.CurrentDate));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


