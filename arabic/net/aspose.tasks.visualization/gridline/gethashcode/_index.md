---
title: "Gridline.GetHashCode"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Gridline. تُعيد قيمة رمز تجزئة للمثيل من فئة Gridline."
type: docs
weight: 60
url: /ar/net/aspose.tasks.visualization/gridline/gethashcode/
---
## Gridline.GetHashCode method

إرجاع قيمة hash code للنسخة من الفئة [`Gridline`](../).

```csharp
public override int GetHashCode()
```

### قيمة الإرجاع

تُرجع قيمة رمز تجزئة لهذا الكائن.

## الأمثلة

يوضح كيفية الحصول على hash code لخط الشبكة.

```csharp
var gridline1 = new Gridline();
var gridline2 = new Gridline();

// hash code لخط الشبكة يعتمد على حقل GUID الداخلي.
Console.WriteLine("Gridline 1 Hash Code: {0}", gridline1.GetHashCode());
Console.WriteLine("Gridline 2 Hash Code: {0}", gridline2.GetHashCode());
```

### انظر أيضًا

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


