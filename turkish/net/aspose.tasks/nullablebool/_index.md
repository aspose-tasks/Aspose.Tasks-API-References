---
title: "Struct NullableBool"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.NullableBool struct. Değerin tanımlanıp tanımlanmadığını kontrol etme imkanı sunan boolean değerler için bir sınıf."
type: docs
weight: 1110
url: /tr/net/aspose.tasks/nullablebool/
---
## NullableBool structure

Değerin tanımlanıp tanımlanmadığını kontrol etme imkanı sunan boolean değerler için bir sınıf.

```csharp
public struct NullableBool : IEquatable<NullableBool>
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [NullableBool](nullablebool/#constructor)(bool) | `NullableBool` struct'ının belirtilen boolean değerle yeni bir örneğini başlatır. |
| [NullableBool](nullablebool/#constructor_1)(bool, bool) | `NullableBool` struct'ının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [IsDefined](../../aspose.tasks/nullablebool/isdefined/) { get; } | Değerin tanımlanıp tanımlanmadığını gösteren bir değer alır; aksi takdirde false. |
| [Value](../../aspose.tasks/nullablebool/value/) { get; set; } | Mevcut değerin true ya da false olduğunu gösteren bir değeri alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Equals](../../aspose.tasks/nullablebool/equals/#equals)(NullableBool) | `NullableBool` sınıfının belirtilen örneğiyle bu örneğin eşit olup olmadığını gösteren bir bayrak döndürür. |
| override [Equals](../../aspose.tasks/nullablebool/equals/#equals_1)(object) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir bayrak döndürür. |
| override [GetHashCode](../../aspose.tasks/nullablebool/gethashcode/)() | `NullableBool` sınıfının örneği için bir hash kod değeri döndürür. |
| override [ToString](../../aspose.tasks/nullablebool/tostring/)() | Geçerli nesneyi temsil eden bir dize döndürür. |
| [operator ==](../../aspose.tasks/nullablebool/op_equality/) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| [implicit operator](../../aspose.tasks/nullablebool/op_implicit/#op_implicit_1) | Bir `NullableBool` örneğini örtülü olarak bir boolean değere dönüştürür. [`Value`](./value/) doğru ve [`IsDefined`](./isdefined/) doğru olduğunda true döndürür. (2 operatör) |
| [operator !=](../../aspose.tasks/nullablebool/op_inequality/) | Bu örneğin belirtilen nesneye eşit olmadığını gösteren bir değer döndürür. |

## Örnekler

&lt;see cref=\"NullableBool\" /&gt; sınıfı ile nasıl çalışılacağını gösterir.

```csharp
var project = new Project();

// <see cref=\"Aspose.Tasks.NullableBool\" /> sınıfının nerede kullanıldığını kontrol edelim
// <see cref=\"Aspose.Tasks.NullableBool\" /> sınıfının temel avantajı
// Birisi, oluşturma yoluyla onu tanımsız olarak ayarlayabilir
var actualsInSync = new NullableBool(false, false);
Console.WriteLine("'ActualsInSync' Value: " + actualsInSync.Value);
Console.WriteLine("'ActualsInSync' Is Defined: " + actualsInSync.IsDefined);

// ...
// nullable bool örneğini kullan
project.Set(Prj.ActualsInSync, actualsInSync);

// ...
var honorConstraints = new NullableBool(true);
Console.WriteLine("'HonorConstraints' ToString: " + honorConstraints.ToString());

// ...
// nullable bool örneğini kullan
project.Set(Prj.HonorConstraints, honorConstraints);

// ...
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


