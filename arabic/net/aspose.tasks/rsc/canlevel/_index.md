---
title: "Rsc.CanLevel"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. يحدد ما إذا كان يمكن إجراء تسوية الموارد على مورد"
type: docs
weight: 200
url: /ar/net/aspose.tasks/rsc/canlevel/
---
## Rsc.CanLevel field

يحدد ما إذا كان يمكن إجراء تسوية الموارد على مورد.

```csharp
public static readonly Key<NullableBool, RscKey> CanLevel;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.CanLevel.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CanLevel, true);

Console.WriteLine("Can Level: " + resource.Get(Rsc.CanLevel));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


