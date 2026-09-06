---
title: "Rsc.Inactive"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Rsc field. يحدد ما إذا تم جعل المورد غير نشط بواسطة مستخدم لديه صلاحيات إدارية"
type: docs
weight: 360
url: /ar/net/aspose.tasks/rsc/inactive/
---
## Rsc.Inactive field

يحدد ما إذا كان المورد قد تم جعله غير نشط بواسطة مستخدم يمتلك صلاحيات إدارية.

```csharp
public static readonly Key<NullableBool, RscKey> Inactive;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Rsc.Inactive.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Inactive, true);

Console.WriteLine("Inactive: " + resource.Get(Rsc.Inactive));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


