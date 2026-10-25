---
title: "Rsc.Code"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Rsc field. الرمز أو معلومات أخرى حول المورد"
type: docs
weight: 210
url: /ar/net/aspose.tasks/rsc/code/
---
## Rsc.Code field

الرمز أو المعلومات الأخرى حول المورد.

```csharp
public static readonly Key<string, RscKey> Code;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Rsc.Code.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Code, "555292");

Console.WriteLine("Code: " + resource.Get(Rsc.Code));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


