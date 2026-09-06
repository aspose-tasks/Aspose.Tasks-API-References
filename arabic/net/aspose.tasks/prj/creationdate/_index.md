---
title: "Prj.CreationDate"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. التاريخ والوقت الذي تم فيه إنشاء المشروع"
type: docs
weight: 130
url: /ar/net/aspose.tasks/prj/creationdate/
---
## Prj.CreationDate field

التاريخ والوقت الذي تم إنشاء المشروع فيه.

```csharp
public static readonly Key<DateTime, PrjKey> CreationDate;
```

## ملاحظات

محفوظ بتنسيق UTC في ملفات mpp. نوع DateTime.

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Prj.CreationDate.

```csharp
var project = new Project();

project.Set(Prj.CreationDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Creation Date: " + project.Get(Prj.CreationDate));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


