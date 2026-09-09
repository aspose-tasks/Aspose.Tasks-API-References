---
title: "Duration.Parse"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Duration yöntemi. Belirtilen dizeyi Duration yapısının örneğine dönüştürür."
type: docs
weight: 10
url: /tr/net/aspose.tasks/duration/parse/
---
## Duration.Parse method

Belirtilen dizeyi [`Duration`](../) yapısının örneğine dönüştürür.

```csharp
public static Duration Parse(Project p, string value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| p | Project | Süreyi dönüştürmek için [`Project`](../../project/) sınıfının belirtilen örneği. |
| value | Dize | dönüştürülecek belirtilen dize. |

### Dönüş Değeri

[`Duration`](../) yapısının dönüştürülmüş örneğini döndürür.

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

* class [Project](../../project/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


