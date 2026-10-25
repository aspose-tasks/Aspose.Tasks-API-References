---
title: "Gridline.Equals"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Gridline. تُعيد علامة تشير إلى ما إذا كان هذا المثيل مساويًا للكائن المحدد."
type: docs
weight: 50
url: /ar/net/aspose.tasks.visualization/gridline/equals/
---
## Gridline.Equals method

يرجع علامة تشير إلى ما إذا كانت هذه المثيلة مساوية للعنصر المحدد.

```csharp
public override bool Equals(object obj)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| obj | كائن | الكائن المحدد للمقارنة بهذه المثيلة. |

### قيمة الإرجاع

علامة تُشير إلى ما إذا كانت هذه المثيلة مساوية للكائن المحدد.

## الأمثلة

يظهر كيفية فحص مساواة خطوط الشبكة.

```csharp
var gridline1 = new Gridline();
var gridline2 = new Gridline();

// يتم فحص مساواة خطوط الشبكة مقابل نوع خط الشبكة.
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Gridline 2 Type: " + gridline2.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));

// غيّر النوع
gridline1.GridlineType = GridlineType.BarRows;
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));
```

### انظر أيضًا

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


