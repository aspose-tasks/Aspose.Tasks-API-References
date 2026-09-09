---
title: "NullableBool.Equals"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "NullableBool yöntemi. Bu örneğin NullableBool sınıfının belirtilen örneğine eşit olup olmadığını gösteren bir bayrak döndürür"
type: docs
weight: 40
url: /tr/net/aspose.tasks/nullablebool/equals/
---
## Equals(NullableBool) {#equals}

Bu örneğin [`NullableBool`](../) sınıfının belirtilen örneğine eşit olup olmadığını gösteren bir bayrak döndürür.

```csharp
public bool Equals(NullableBool other)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| diğer | NullableBool | bu örnek ile karşılaştırılacak belirtilen nesne. |

### Dönüş Değeri

Bu örneğin [`NullableBool`](../) sınıfının belirtilen örneğine eşit olup olmadığını gösteren bir bayrak.

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

## Equals(object) {#equals_1}

Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir bayrak döndürür.

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object | bu örnek ile karşılaştırılacak belirtilen nesne. |

### Dönüş Değeri

bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir bayrak.

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


