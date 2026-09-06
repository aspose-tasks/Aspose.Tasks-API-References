---
title: "NullableBool.Equals"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة NullableBool. تُرجع علامة تشير إلى ما إذا كان هذا الكائن مساويًا للنسخة المحددة من فئة NullableBool."
type: docs
weight: 40
url: /ar/net/aspose.tasks/nullablebool/equals/
---
## Equals(NullableBool) {#equals}

تُرجع علامة تشير إلى ما إذا كان هذا الكائن مساويًا للنسخة المحددة من فئة [`NullableBool`](../).

```csharp
public bool Equals(NullableBool other)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| آخر | NullableBool | الكائن المحدد للمقارنة بهذه المثيلة. |

### قيمة الإرجاع

علامة تشير إلى ما إذا كان هذا الكائن مساويًا للنسخة المحددة من فئة [`NullableBool`](../).

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

---

## Equals(object) {#equals_1}

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


