---
title: "Sınıf RiskItemStatistics"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.RiskAnalysis.RiskItemStatistics sınıfı. Analiz edilen projenin görevine ait istatistiksel verileri depolayan bir öğeyi temsil eder."
type: docs
weight: 1900
url: /tr/net/aspose.tasks.riskanalysis/riskitemstatistics/
---
## RiskItemStatistics class

Analiz edilen projenin görevi için istatistiksel verileri depolayan bir öğeyi temsil eder.

```csharp
public class RiskItemStatistics
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ExpectedValue](../../aspose.tasks.riskanalysis/riskitemstatistics/expectedvalue/) { get; } | Risk öğesinin beklenen değerini alır. |
| [ItemType](../../aspose.tasks.riskanalysis/riskitemstatistics/itemtype/) { get; } | [`RiskItemType`](../riskitemtype/) enum'ının bir örneğini alır. |
| [Maximum](../../aspose.tasks.riskanalysis/riskitemstatistics/maximum/) { get; } | Monte Carlo simülasyonu sırasında üretilen maksimum değeri alır. |
| [Minimum](../../aspose.tasks.riskanalysis/riskitemstatistics/minimum/) { get; } | Monte Carlo simülasyonu sırasında üretilen minimum değeri alır. |
| [StandardDeviation](../../aspose.tasks.riskanalysis/riskitemstatistics/standarddeviation/) { get; } | Risk öğesinin standart sapmasını alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetPercentile](../../aspose.tasks.riskanalysis/riskitemstatistics/getpercentile/)(int) | Üretilen örneklerin belirli bir yüzdesinin altında kalan bir değeri alır. |
| override [ToString](../../aspose.tasks.riskanalysis/riskitemstatistics/tostring/)() | Risk öğesinin kısa metin temsilini döndürür. Temsilin tam detayları belirtilmemiştir ve değişebilir. |

## Örnekler

Risk istatistiklerinin nasıl hesaplanacağını gösterir.

```csharp
var settings = new RiskAnalysisSettings
{
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// Risk desenini başlat
var pattern = new RiskPattern(task)
{
    // Rastgele sayı üreteci için olası değerleri oluşturacak dağılım tipini seçin (şu anda yalnızca iki tip desteklenmektedir: normal ve uniform)
    // Daha fazla ayrıntı için buraya bakın: https://en.wikipedia.org/wiki/Normal_distribution)
    Distribution = ProbabilityDistributionType.Normal,

    // En olası görev süresinin, en iyi proje senaryosunda gerçekleşebilecek yüzde oranını ayarlayın
    // Varsayılan değer 75'tir, bu da tahmini belirtilen görev süresi 4 gün ise iyimser sürenin 3 gün olacağı anlamına gelir
    Optimistic = 70,

    // En olası görev süresinin, en kötü proje senaryosunda gerçekleşebilecek yüzde oranını ayarlayın
    // Varsayılan değer 125'tir, bu da tahmini belirtilen görev süresi 4 gün ise kötümser sürenin 5 gün olacağı anlamına gelir
    Pessimistic = 130,

    // İyimser ve kötümser tahminler arasında gerçek değerlerin bulunacağı zaman yüzdesine karşılık gelen bir güven düzeyi ayarlayın
    // Bunu standart sapma değeri olarak düşünebilirsiniz: tahminleriniz ne kadar belirsizse, rastgele sayı üretecinde kullanılan standart sapma değeri de o kadar yüksek olur
    ConfidenceLevel = ConfidenceLevel.CL75
};
settings.Patterns.Add(pattern);

// Proje risklerini analiz edin
var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);
var statistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Short statistic: " + statistics);
Console.WriteLine();
Console.WriteLine("Statistic details: ");
Console.WriteLine("Item Type: {0}", statistics.ItemType);
Console.WriteLine("Expected value: {0}", statistics.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", statistics.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", statistics.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", statistics.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", statistics.GetPercentile(90));
Console.WriteLine("Minimum: {0}", statistics.Minimum);
Console.WriteLine("Maximum: {0}", statistics.Maximum);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


