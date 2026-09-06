---
title: "Rsc.MaterialLabel"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. وحدة القياس للمورد المادي"
type: docs
weight: 440
url: /ar/net/aspose.tasks/rsc/materiallabel/
---
## Rsc.MaterialLabel field

وحدة القياس للمورد المادي.

```csharp
public static readonly Key<string, RscKey> MaterialLabel;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.MaterialLabel.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaterialLabel, "kg");

Console.WriteLine("Material Label: " + resource.Get(Rsc.MaterialLabel));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


