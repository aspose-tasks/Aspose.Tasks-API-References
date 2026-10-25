---
title: "NullableBool.op_Implicit"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة NullableBool. تقوم بتحويل كائن NullableBool إلى قيمة منطقية ضمنيًا. تُعيد true عندما تكون Value true و IsDefined true."
type: docs
weight: 80
url: /ar/net/aspose.tasks/nullablebool/op_implicit/
---
## implicit operator {#op_implicit_1}

تحول ضمنيًا كائن [`NullableBool`](../) إلى قيمة منطقية. تُعيد true عندما يكون [`Value`](../value/) true و [`IsDefined`](../isdefined/) true.

```csharp
public static implicit operator bool(NullableBool val)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| القيمة | NullableBool | القيمة المراد تحويلها. |

### قيمة الإرجاع

قيمة منطقية.

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

## implicit operator {#op_implicit}

يقوم بتحويل قيمة منطقية إلى كائن [`NullableBool`](../) ضمنيًا.

```csharp
public static implicit operator NullableBool(bool val)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| القيمة | Boolean | القيمة للتحويل. |

### قيمة الإرجاع

كائن [`NullableBool`](../) محوَّل.

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


