---
title: "NullableBool.op_Inequality"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة NullableBool. تُرجع قيمة تشير إلى ما إذا كان هذا الكائن غير مساوي لكائن محدد."
type: docs
weight: 90
url: /ar/net/aspose.tasks/nullablebool/op_inequality/
---
## NullableBool Inequality operator

يعيد قيمة تشير إلى ما إذا كانت هذه الحالة غير مساوية لكائن محدد.

```csharp
public static bool operator !=(NullableBool a, NullableBool b)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| a | NullableBool | الأول [`NullableBool`](../). |
| b | NullableBool | الثاني [`NullableBool`](../). |

### قيمة الإرجاع

قيمة تشير إلى ما إذا كانت هذه المثيلة غير مساوية لكائن محدد

## الأمثلة

Shows how to compare &lt;see cref=\"Aspose.Tasks.NullableBool\" /&gt; instances.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// يتم فحص مساواة القيم المنطقية مقابل خصائص 'IsDefined' و 'Value'.
Console.WriteLine("Nullable Bool 1: " + bool1.ToString());
Console.WriteLine("Nullable Bool 2: " + bool2.ToString());

// يفحص التحويل الضمني إلى bool: bool1 هو True لأنه معرف وتم تعيين Value إلى True.
if (bool1)
{
    Console.WriteLine("Nullable Bool 1 is True");
}
else
{
    Console.WriteLine("Nullable Bool 1 is False");
}

// يفحص التحويل الضمني إلى bool: bool2 هو False لأنه غير معرف.
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}

Console.WriteLine("Are bools equal: " + bool1.Equals(bool2));

// يفحص التحويل الضمني إلى bool
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}
```

### انظر أيضًا

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


