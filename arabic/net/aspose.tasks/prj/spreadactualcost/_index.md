---
title: "Prj.SpreadActualCost"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. يحدد ما إذا كانت التكاليف الفعلية موزعة إلى تاريخ الحالة"
type: docs
weight: 660
url: /ar/net/aspose.tasks/prj/spreadactualcost/
---
## Prj.SpreadActualCost field

يحدد ما إذا كانت التكاليف الفعلية تُوزّع إلى تاريخ الحالة.

```csharp
public static readonly Key<NullableBool, PrjKey> SpreadActualCost;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Prj.SpreadActualCost.

```csharp
var project = new Project();

project.Set(Prj.SpreadActualCost, true);

Console.WriteLine("Spread Actual Cost: " + project.Get(Prj.SpreadActualCost));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


