---
title: "Rsc.IsNull"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. يحدد ما إذا كان المورد null"
type: docs
weight: 420
url: /ar/net/aspose.tasks/rsc/isnull/
---
## Rsc.IsNull field

يحدد ما إذا كان المورد فارغًا.

```csharp
public static readonly Key<NullableBool, RscKey> IsNull;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Rsc.IsNull.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsNull, true);

Console.WriteLine("Is Null: " + resource.Get(Rsc.IsNull));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


