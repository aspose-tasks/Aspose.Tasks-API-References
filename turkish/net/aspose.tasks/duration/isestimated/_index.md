---
title: "Duration.IsEstimated"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Duration özelliği. Zaman biriminin tahmini olup olmadığını gösteren bir değer alır. Bu Duration örneğinin tahmini olup olmadığını belirleyen bayrak."
type: docs
weight: 30
url: /tr/net/aspose.tasks/duration/isestimated/
---
## Duration.IsEstimated property

Zaman biriminin tahmini olup olmadığını gösteren bir değer alır. Bu Duration örneğinin tahmini olup olmadığını belirleyen bayrak.

```csharp
public bool IsEstimated { get; }
```

## Örnekler

Özel biçimlendirilmiş bir stringden nasıl string ayrıştırılacağını gösterir.

```csharp
var project = new Project();

// süre örnekleri:
// "1d", "1dy", "1d?", "1day", "1 dy", "1 edy? ", "8hr", "8 hour", "8hours", "0.2w?", "0.2wk", "0.2 eweek", "0.2ew?"
// burada 1 - öğe sayısı (gün, hafta, vb), d - gün (h - saat, w - hafta) ? - tahmini bayrak, e - geçen bayrak

// tahmini bir süreyi ayrıştırmayı deneyin
var duration1 = Duration.Parse(project, "1d?");
Console.WriteLine("The parsed time span: " + duration1.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration1.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration1.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration1.IsElapsed);
Console.WriteLine();

// tahmini bir süreyi ayrıştırmayı deneyin
var duration2 = Duration.Parse(project, "0.2 eweek");
Console.WriteLine("The parsed time span: " + duration2.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration2.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration2.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration2.IsElapsed);
```

### Ayrıca Bakınız

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


