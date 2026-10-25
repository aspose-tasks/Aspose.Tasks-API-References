---
title: "Rsc.IsEnterprise"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. يوضح ما إذا كان المورد من مجموعة موارد المؤسسة (true) أو من مجموعة الموارد المحلية (false)"
type: docs
weight: 400
url: /ar/net/aspose.tasks/rsc/isenterprise/
---
## Rsc.IsEnterprise field

يعرض ما إذا كان المورد من مجموعة موارد المؤسسة (صحيح) أو من مجموعة الموارد المحلية (خطأ).

```csharp
public static readonly Key<NullableBool, RscKey> IsEnterprise;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Rsc.IsEnterprise.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsEnterprise, true);

Console.WriteLine("Is Enterprise: " + resource.Get(Rsc.IsEnterprise));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


