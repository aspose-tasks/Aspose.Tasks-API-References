---
title: "Rsc.Initials"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. الأحرف الأولى للمورد"
type: docs
weight: 370
url: /ar/net/aspose.tasks/rsc/initials/
---
## Rsc.Initials field

الأحرف الأولى للمورد.

```csharp
public static readonly Key<string, RscKey> Initials;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.Initials.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Initials, "R");

Console.WriteLine("Initials: " + resource.Get(Rsc.Initials));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


