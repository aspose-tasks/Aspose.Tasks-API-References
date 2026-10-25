---
title: "Rsc.Type"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. نوع المورد"
type: docs
weight: 660
url: /ar/net/aspose.tasks/rsc/type/
---
## Rsc.Type field

نوع المورد.

```csharp
public static readonly Key<ResourceType, RscKey> Type;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Rsc.Type.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Type, ResourceType.Work);

Console.WriteLine("Type: " + resource.Get(Rsc.Type));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [ResourceType](../../resourcetype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


