---
title: "Prj.EarnedValueMethod"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. الطريقة الافتراضية لحساب القيمة المكتسبة"
type: docs
weight: 310
url: /ar/net/aspose.tasks/prj/earnedvaluemethod/
---
## Prj.EarnedValueMethod field

طريقة حساب القيمة المكتسبة الافتراضية.

```csharp
public static readonly Key<EarnedValueMethodType, PrjKey> EarnedValueMethod;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Prj.EarnedValueMethod.

```csharp
var project = new Project();

project.Set(Prj.EarnedValueMethod, EarnedValueMethodType.PhysicalPercentComplete);

Console.WriteLine("Earned Value Method: " + project.Get(Prj.EarnedValueMethod));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


