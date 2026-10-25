---
title: "Rsc.IsCostResource"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. يحدد ما إذا كان المورد مورد تكلفة"
type: docs
weight: 390
url: /ar/net/aspose.tasks/rsc/iscostresource/
---
## Rsc.IsCostResource field

يحدد ما إذا كان المورد هو مورد تكلفة.

```csharp
public static readonly Key<NullableBool, RscKey> IsCostResource;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.IsCostResource.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsCostResource, true);

Console.WriteLine("Is Cost Resource: " + resource.Get(Rsc.IsCostResource));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


