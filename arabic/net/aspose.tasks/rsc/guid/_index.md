---
title: "Rsc.Guid"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. يحتوي على رمز التعريف الفريد المُولد للمورد"
type: docs
weight: 310
url: /ar/net/aspose.tasks/rsc/guid/
---
## Rsc.Guid field

يحتوي على رمز التعريف الفريد المُولد للمورد.

```csharp
public static readonly Key<string, RscKey> Guid;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Rsc.Guid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Guid, "1385689c-2dd1-4114-935b-054beb6fbbbe");

Console.WriteLine("Guid: " + resource.Get(Rsc.Guid));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


