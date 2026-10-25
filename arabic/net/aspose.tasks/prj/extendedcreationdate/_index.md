---
title: "Prj.ExtendedCreationDate"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. التاريخ المستخدم للحساب والتقارير"
type: docs
weight: 320
url: /ar/net/aspose.tasks/prj/extendedcreationdate/
---
## Prj.ExtendedCreationDate field

التاريخ المستخدم للحساب والتقارير.

```csharp
public static readonly Key<DateTime, PrjKey> ExtendedCreationDate;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Prj.ExtendedCreationDate.

```csharp
var project = new Project();

project.Set(Prj.ExtendedCreationDate, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Extended Creation Date: " + project.Get(Prj.ExtendedCreationDate));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


