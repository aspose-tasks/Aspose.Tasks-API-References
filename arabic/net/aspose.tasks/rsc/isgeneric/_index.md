---
title: "Rsc.IsGeneric"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. يحدد ما إذا كان المورد عامًا أم لا"
type: docs
weight: 410
url: /ar/net/aspose.tasks/rsc/isgeneric/
---
## Rsc.IsGeneric field

يحدد ما إذا كان المورد عامًا أم لا.

```csharp
public static readonly Key<NullableBool, RscKey> IsGeneric;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.IsGeneric.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsGeneric, true);

Console.WriteLine("Is Generic: " + resource.Get(Rsc.IsGeneric));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


