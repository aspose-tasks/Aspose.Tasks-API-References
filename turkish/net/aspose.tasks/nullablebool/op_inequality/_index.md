---
title: "NullableBool.op_Inequality"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "NullableBool yöntemi. Bu örneğin belirtilen bir nesneye eşit olmaması durumunu gösteren bir değer döndürür"
type: docs
weight: 90
url: /tr/net/aspose.tasks/nullablebool/op_inequality/
---
## NullableBool Inequality operator

Bu örneğin belirtilen nesneye eşit olmadığını gösteren bir değer döndürür.

```csharp
public static bool operator !=(NullableBool a, NullableBool b)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | NullableBool | İlk [`NullableBool`](../) örneği. |
| b | NullableBool | İkinci [`NullableBool`](../) örneği. |

### Dönüş Değeri

Bu örneğin belirtilen bir nesneye eşit olup olmadığını gösteren bir değer

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


