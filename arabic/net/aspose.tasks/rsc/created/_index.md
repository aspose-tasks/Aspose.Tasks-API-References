---
title: "Rsc.Created"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. التاريخ والوقت عندما تم إضافة مورد إلى المشروع"
type: docs
weight: 260
url: /ar/net/aspose.tasks/rsc/created/
---
## Rsc.Created field

التاريخ والوقت الذي تم فيه إضافة المورد إلى المشروع.

```csharp
public static readonly Key<DateTime, RscKey> Created;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.Created.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + resource.Get(Rsc.Created));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


