---
title: "Rsc.Name"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. اسم المورد"
type: docs
weight: 460
url: /ar/net/aspose.tasks/rsc/name/
---
## Rsc.Name field

اسم المورد.

```csharp
public static readonly Key<string, RscKey> Name;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Rsc.Name.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Name, "John Smith");

Console.WriteLine("Name: " + resource.Get(Rsc.Name));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


