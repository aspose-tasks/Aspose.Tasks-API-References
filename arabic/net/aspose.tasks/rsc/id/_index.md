---
title: "Rsc.Id"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. معرف الموقع للمورد ضمن قائمة الموارد"
type: docs
weight: 350
url: /ar/net/aspose.tasks/rsc/id/
---
## Rsc.Id field

معرف الموضع للمورد ضمن قائمة الموارد.

```csharp
public static readonly Key<int, RscKey> Id;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.Id.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Id, 987);

Console.WriteLine("Id: " + resource.Get(Rsc.Id));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


