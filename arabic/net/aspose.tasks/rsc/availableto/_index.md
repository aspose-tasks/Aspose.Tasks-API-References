---
title: "Rsc.AvailableTo"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. تاريخ الانتهاء الذي يكون فيه المورد متاحًا للعمل بالوحدات المحددة للفترة الزمنية الحالية"
type: docs
weight: 130
url: /ar/net/aspose.tasks/rsc/availableto/
---
## Rsc.AvailableTo field

تاريخ الانتهاء الذي يكون فيه المورد متاحًا للعمل بالوحدات المحددة للفترة الزمنية الحالية.

```csharp
public static readonly Key<DateTime, RscKey> AvailableTo;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.AvailableTo.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableTo, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available To: " + resource.Get(Rsc.AvailableTo));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


