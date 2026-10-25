---
title: "NullableBool.op_Implicit"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "NullableBool yöntemi. Bir NullableBool örneğini örtük olarak bir boolean değere dönüştürür. Value true ve IsDefined true olduğunda true döndürür"
type: docs
weight: 80
url: /tr/net/aspose.tasks/nullablebool/op_implicit/
---
## implicit operator {#op_implicit_1}

Bir [`NullableBool`](../) örneğini örtük olarak bir boolean değere dönüştürür. [`Value`](../value/) true ve [`IsDefined`](../isdefined/) true olduğunda true döndürür.

```csharp
public static implicit operator bool(NullableBool val)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| val | NullableBool | Dönüştürülecek değer. |

### Dönüş Değeri

bir boolean değer.

## Örnekler

Nasıl karşılaştırılacağını gösterir &lt;see cref="Aspose.Tasks.NullableBool" /&gt; örneklerini.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// bool'ların eşitliği 'IsDefined' ve 'Value' özelliklerine karşı kontrol edilir.
Console.WriteLine("Nullable Bool 1: " + bool1.ToString());
Console.WriteLine("Nullable Bool 2: " + bool2.ToString());

// örtük dönüşümünü bool'a kontrol eder: bool1 tanımlı olduğu ve Value True olarak ayarlandığı için True'dır.
if (bool1)
{
    Console.WriteLine("Nullable Bool 1 is True");
}
else
{
    Console.WriteLine("Nullable Bool 1 is False");
}

// örtük dönüşümünü bool'a kontrol eder: bool2 tanımlı olmadığı için False'tır.
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}

Console.WriteLine("Are bools equal: " + bool1.Equals(bool2));

// örtük dönüşümünü bool'a kontrol eder
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}
```

### Ayrıca Bakınız

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)

---

## implicit operator {#op_implicit}

Boolean değeri [`NullableBool`](../) örneğine örtük olarak dönüştürür.

```csharp
public static implicit operator NullableBool(bool val)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| val | Boolean | Dönüştürülecek değer. |

### Dönüş Değeri

Dönüştürülmüş [`NullableBool`](../) örneği.

## Örnekler

Nasıl karşılaştırılacağını gösterir &lt;see cref="Aspose.Tasks.NullableBool" /&gt; örneklerini.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// bool'ların eşitliği 'IsDefined' ve 'Value' özelliklerine karşı kontrol edilir.
Console.WriteLine("Nullable Bool 1: " + bool1.ToString());
Console.WriteLine("Nullable Bool 2: " + bool2.ToString());

// örtük dönüşümünü bool'a kontrol eder: bool1 tanımlı olduğu ve Value True olarak ayarlandığı için True'dır.
if (bool1)
{
    Console.WriteLine("Nullable Bool 1 is True");
}
else
{
    Console.WriteLine("Nullable Bool 1 is False");
}

// örtük dönüşümünü bool'a kontrol eder: bool2 tanımlı olmadığı için False'tır.
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}

Console.WriteLine("Are bools equal: " + bool1.Equals(bool2));

// örtük dönüşümünü bool'a kontrol eder
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}
```

### Ayrıca Bakınız

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


