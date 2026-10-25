---
title: "Sınıf RiskPattern"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.RiskAnalysis.RiskPattern sınıfı. Bir proje görevine ait risk desenini temsil eder."
type: docs
weight: 1930
url: /tr/net/aspose.tasks.riskanalysis/riskpattern/
---
## RiskPattern class

Bir proje görevi için risk desenini temsil eder.

```csharp
public class RiskPattern
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [RiskPattern](riskpattern/)(Task) | `RiskPattern` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ConfidenceLevel](../../aspose.tasks.riskanalysis/riskpattern/confidencelevel/) { get; set; } | Gerçek üretilen değerlerin iyimser ve kötümser tahminler içinde kalacağı zaman yüzdesine karşılık gelen güven düzeyini alır veya ayarlar. Varsayılan değer CL99'dur. |
| [Distribution](../../aspose.tasks.riskanalysis/riskpattern/distribution/) { get; set; } | Monte Carlo simülasyonunda kullanılan olasılık dağılımını alır veya ayarlar. Varsayılan değer ProbabilityDistributionType.Normal'dur. |
| [Optimistic](../../aspose.tasks.riskanalysis/riskpattern/optimistic/) { get; set; } | En iyi olası proje senaryosunda gerçekleşebilecek en muhtemel görev süresinin yüzdesini alır veya ayarlar. Varsayılan değer 75'tir, bu da tahmini görev süresi 4 gün ise iyimser sürenin 3 gün olacağı anlamına gelir. |
| [Pessimistic](../../aspose.tasks.riskanalysis/riskpattern/pessimistic/) { get; set; } | En kötü olası proje senaryosunda gerçekleşebilecek en muhtemel görev süresinin yüzdesini alır veya ayarlar. Varsayılan değer 125'tir, bu da tahmini görev süresi 4 gün ise kötümser sürenin 5 gün olacağı anlamına gelir. |
| [Task](../../aspose.tasks.riskanalysis/riskpattern/task/) { get; } | Bu risk deseninin uygulandığı proje görevini alır. |

## Örnekler

Risk simülasyonu ayarlarının nasıl tanımlanacağını gösterir.

```csharp
var settings = new RiskAnalysisSettings();
settings.IterationsCount = 200;

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// Risk desenini başlat
var pattern = new RiskPattern(task);

// Rastgele sayı üreteci için olası değerleri oluşturacak dağılım tipini seçin (şu anda yalnızca iki tip desteklenmektedir: normal ve uniform)
// Daha fazla ayrıntı için buraya bakın: https://en.wikipedia.org/wiki/Normal_distribution)
pattern.Distribution = ProbabilityDistributionType.Normal;

// En olası görev süresinin, en iyi proje senaryosunda gerçekleşebilecek yüzde oranını ayarlayın
// Varsayılan değer 75'tir, bu da tahmini belirtilen görev süresi 4 gün ise iyimser sürenin 3 gün olacağı anlamına gelir
pattern.Optimistic = 70;

// En olası görev süresinin, en kötü proje senaryosunda gerçekleşebilecek yüzde oranını ayarlayın
// Varsayılan değer 125'tir, bu da tahmini belirtilen görev süresi 4 gün ise kötümser sürenin 5 gün olacağı anlamına gelir
pattern.Pessimistic = 130;

// İyimser ve kötümser tahminler arasında gerçek değerlerin bulunacağı zaman yüzdesine karşılık gelen bir güven düzeyi ayarlayın
// Bunu standart sapma değeri olarak düşünebilirsiniz: tahminleriniz ne kadar belirsizse, rastgele sayı üretecinde kullanılan standart sapma değeri de o kadar yüksek olur
pattern.ConfidenceLevel = ConfidenceLevel.CL75;

settings.Patterns.Add(pattern);

var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);
var earlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", earlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", earlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", earlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", earlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", earlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", earlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", earlyFinish.Maximum);

analysisResult.SaveReport(OutDir + "AnalysisReport_out.pdf");
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


