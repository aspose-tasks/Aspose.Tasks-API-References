---
title: "Rsc.AvailableFrom"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. تاريخ البدء الذي يكون فيه المورد متاحًا للعمل بالوحدات المحددة للفترة الزمنية الحالية"
type: docs
weight: 120
url: /ar/net/aspose.tasks/rsc/availablefrom/
---
## Rsc.AvailableFrom field

تاريخ البدء الذي يكون فيه المورد متاحًا للعمل بالوحدات المحددة للفترة الزمنية الحالية.

```csharp
public static readonly Key<DateTime, RscKey> AvailableFrom;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.AvailableFrom.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableFrom, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available From: " + resource.Get(Rsc.AvailableFrom));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


