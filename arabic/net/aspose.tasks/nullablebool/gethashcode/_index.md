---
title: "NullableBool.GetHashCode"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة NullableBool. تُرجع قيمة تجزئة (hash code) للنسخة من فئة NullableBool."
type: docs
weight: 50
url: /ar/net/aspose.tasks/nullablebool/gethashcode/
---
## NullableBool.GetHashCode method

تُرجع قيمة تجزئة للنسخة من فئة [`NullableBool`](../).

```csharp
public override int GetHashCode()
```

### قيمة الإرجاع

تُرجع قيمة رمز تجزئة لهذا الكائن.

## الأمثلة

يظهر كيفية العمل مع طريقة &lt;see cref="Aspose.Tasks.NullableBool" /&gt;.GetHashCode.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// قيمة التجزئة للمتغيرات المنطقية تستند إلى خصائص 'IsDefined' و 'Value'.
Console.WriteLine("Bool 1: {0} Hash Code 1: {1}", bool1.ToString(), bool1.GetHashCode());
Console.WriteLine("Bool 2: {0} Hash Code 1: {1}", bool2.ToString(), bool2.GetHashCode());
```

### انظر أيضًا

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


