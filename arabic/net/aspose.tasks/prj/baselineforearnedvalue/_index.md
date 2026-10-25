---
title: "Prj.BaselineForEarnedValue"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. الخط الأساسي المحدد المستخدم لحساب قيم التباين"
type: docs
weight: 80
url: /ar/net/aspose.tasks/prj/baselineforearnedvalue/
---
## Prj.BaselineForEarnedValue field

الخط الأساسي المحدد المستخدم لحساب قيم التباين.

```csharp
public static readonly Key<BaselineType, PrjKey> BaselineForEarnedValue;
```

## الأمثلة

يظهر كيفية قراءة/كتابة خاصية Prj.BaselineForEarnedValue.

```csharp
var project = new Project();

project.Set(Prj.BaselineForEarnedValue, BaselineType.Baseline);

Console.WriteLine("Baseline For Earned Value: " + project.Get(Prj.BaselineForEarnedValue));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BaselineType](../../baselinetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


