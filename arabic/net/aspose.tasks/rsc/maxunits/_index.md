---
title: "Rsc.MaxUnits"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. الحد الأقصى لعدد الوحدات التي تمثل السعة القصوى التي يتوفر فيها المورد لإنجاز أي مهام خلال الفترة الزمنية الحالية"
type: docs
weight: 450
url: /ar/net/aspose.tasks/rsc/maxunits/
---
## Rsc.MaxUnits field

الحد الأقصى لعدد الوحدات التي تمثل السعة القصوى التي يكون المورد متاحًا لإنجاز أي مهام خلالها في الفترة الزمنية الحالية.

```csharp
public static readonly Key<double, RscKey> MaxUnits;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.MaxUnits.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaxUnits, 2);

Console.WriteLine("Max Units: " + resource.Get(Rsc.MaxUnits));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


