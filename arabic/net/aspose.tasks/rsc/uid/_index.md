---
title: "Rsc.Uid"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. المعرف الفريد لمورد"
type: docs
weight: 670
url: /ar/net/aspose.tasks/rsc/uid/
---
## Rsc.Uid field

المعرّف الفريد للمورد.

```csharp
public static readonly Key<int, RscKey> Uid;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Rsc.Uid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Uid, 99);

Console.WriteLine("Uid: " + resource.Get(Rsc.Uid));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


