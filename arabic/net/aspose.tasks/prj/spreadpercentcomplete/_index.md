---
title: "Prj.SpreadPercentComplete"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. يحدد ما إذا كانت النسبة المكتملة تُوزَّع إلى تاريخ الحالة"
type: docs
weight: 670
url: /ar/net/aspose.tasks/prj/spreadpercentcomplete/
---
## Prj.SpreadPercentComplete field

يحدد ما إذا كان نسبة الإنجاز تُوزّع إلى تاريخ الحالة.

```csharp
public static readonly Key<NullableBool, PrjKey> SpreadPercentComplete;
```

## الأمثلة

يُظهر كيفية قراءة/كتابة خاصية Prj.SpreadPercentComplete.

```csharp
var project = new Project();

project.Set(Prj.SpreadPercentComplete, true);

Console.WriteLine("Spread Percent Complete: " + project.Get(Prj.SpreadPercentComplete));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


