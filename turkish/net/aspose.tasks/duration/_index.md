---
title: Struct Duration
second_title: Aspose.Tasks for .NET API Referansı
description: Aspose.Tasks.Duration yapı. Bir projedeki süreyi temsil eder.
type: docs
weight: 470
url: /tr/net/aspose.tasks/duration/
---
## Duration structure

Bir projedeki süreyi temsil eder.

```csharp
public struct Duration : IEquatable<Duration>
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [IsElapsed](../../aspose.tasks/duration/iselapsed/) { get; } | Zaman biriminin geçip geçmediğini gösteren bir değer alır. Bu Duration örneğinin geçip geçmediğini belirleyen bayrak. |
| [IsEstimated](../../aspose.tasks/duration/isestimated/) { get; } | Zaman biriminin tahmin edilip edilmediğini gösteren bir değer alır. Bu Duration örneğinin tahmin edilip edilmediğini belirleyen bayrak. |
| [TimeSpan](../../aspose.tasks/duration/timespan/) { get; } | Alır[`TimeSpan`](./timespan/) bu Süre nesnesinin örneği. Bu Duration nesnesinin TimeSpan örneği. |
| [TimeUnit](../../aspose.tasks/duration/timeunit/) { get; } | Bu nesne için zaman birimi türünü alır. Bu Duration örneğinin zaman birimi türü. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| static [Parse](../../aspose.tasks/duration/parse/)(Project, string) | Belirtilen dizgiyi örneğine dönüştürür`Duration` yapı. |
| [Add](../../aspose.tasks/duration/add/#add_1)(double) | Bu süreye belirtilen çift değeri ekler. |
| [Add](../../aspose.tasks/duration/add/#add)(Duration) | Belirtilen süreyi bu süreye ekler. |
| [Convert](../../aspose.tasks/duration/convert/)(TimeUnitType) | Süre nesnesini belirtilen zaman birimleriyle başka bir süreye dönüştürür. |
| [Equals](../../aspose.tasks/duration/equals/#equals)(Duration) | Bu örneğin belirtilen bir nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| override [Equals](../../aspose.tasks/duration/equals/#equals_1)(object) | Bu örneğin belirtilen bir nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| override [GetHashCode](../../aspose.tasks/duration/gethashcode/)() | Bu nesne için bir karma kod değeri döndürür. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract_1)(double) | Belirtilen çift değeri bu süre örneğinden çıkarır. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract)(Duration) | Belirtilen süreyi bu süre örneğinden çıkarır. |
| [ToDouble](../../aspose.tasks/duration/todouble/)() | Süre nesnesini şuna dönüştürür:Double değer. |
| override [ToString](../../aspose.tasks/duration/tostring/)() | Bu örneğin dize gösterimini döndürür. |
| static [ParseTimeSpan](../../aspose.tasks/duration/parsetimespan/)(string) | Süre dizesini "PT--H--M--S--" biçiminde ayrıştırır. |
| [operator ==](../../aspose.tasks/duration/op_equality/) | Bu örneğin belirtilen bir nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| [operator !=](../../aspose.tasks/duration/op_inequality/) | Bu örneğin belirtilen bir nesneye eşit olup olmadığını gösteren bir değer döndürür. |

### Ayrıca bakınız

* ad alanı [Aspose.Tasks](../../aspose.tasks/)
* toplantı [Aspose.Tasks](../../)


