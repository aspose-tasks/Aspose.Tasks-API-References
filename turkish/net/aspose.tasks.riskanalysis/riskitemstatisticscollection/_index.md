---
title: "Sınıf RiskItemStatisticsCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.RiskAnalysis.RiskItemStatisticsCollection sınıfı. RiskItemStatistics sınıfının örneklerini içeren bir koleksiyonu temsil eder"
type: docs
weight: 1910
url: /tr/net/aspose.tasks.riskanalysis/riskitemstatisticscollection/
---
## RiskItemStatisticsCollection class

[`RiskItemStatistics`](../riskitemstatistics/) sınıfının örneklerini içeren bir koleksiyonu temsil eder.

```csharp
public class RiskItemStatisticsCollection : IDictionary<Task, RiskItemStatistics>, 
    IEnumerable<RiskItemStatistics>
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Get](../../aspose.tasks.riskanalysis/riskitemstatisticscollection/get/)(Task) | Bu koleksiyonda bulunan ve belirtilen Görev nesnesiyle ilişkili olan [`RiskItemStatistics`](../riskitemstatistics/) sınıfının bir örneğini döndürür; öğe bulunamazsa null döner. |
| [GetEnumerator](../../aspose.tasks.riskanalysis/riskitemstatisticscollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |

## Örnekler

Risk istatistikleri koleksiyonu ile nasıl çalışılacağını gösterir.

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

var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);

// tüm istatistik öğeleri üzerinde yineleme yapın
var statistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish);

foreach (var statistic in statistics)
{
    Console.WriteLine("Short statistic: " + statistic);
    Console.WriteLine();
    Console.WriteLine("Statistic details: ");
    Console.WriteLine("Item Type: {0}", statistic.ItemType);
    Console.WriteLine("Expected value: {0}", statistic.ExpectedValue);
    Console.WriteLine("StandardDeviation: {0}", statistic.StandardDeviation);
    Console.WriteLine("10% Percentile: {0}", statistic.GetPercentile(10));
    Console.WriteLine("50% Percentile: {0}", statistic.GetPercentile(50));
    Console.WriteLine("90% Percentile: {0}", statistic.GetPercentile(90));
    Console.WriteLine("Minimum: {0}", statistic.Minimum);
    Console.WriteLine("Maximum: {0}", statistic.Maximum);
}

// veya belirli bir istatistik alın
var itemStatistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Print the specific statistic: ");
Console.WriteLine("Expected value: {0}", itemStatistics.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", itemStatistics.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", itemStatistics.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", itemStatistics.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", itemStatistics.GetPercentile(90));
Console.WriteLine("Minimum: {0}", itemStatistics.Minimum);
Console.WriteLine("Maximum: {0}", itemStatistics.Maximum);
```

### Ayrıca Bakınız

* class [Task](../../aspose.tasks/task/)
* class [RiskItemStatistics](../riskitemstatistics/)
* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


