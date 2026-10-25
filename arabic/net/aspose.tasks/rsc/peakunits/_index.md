---
title: "Rsc.PeakUnits"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. الحد الأقصى لوحدة التعيين لمورد في أي لحظة زمنية لجميع المهام التي يُعيّن إليها المورد"
type: docs
weight: 540
url: /ar/net/aspose.tasks/rsc/peakunits/
---
## Rsc.PeakUnits field

وحدة التعيين القصوى للمورد في أي لحظة زمنية لجميع المهام التي تم تعيين المورد لها.

```csharp
public static readonly Key<double, RscKey> PeakUnits;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.PeakUnits.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.PeakUnits, 2);

Console.WriteLine("Peak Units: " + resource.Get(Rsc.PeakUnits));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


