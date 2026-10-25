---
title: "Sınıf RiskAnalyzer"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.RiskAnalysis.RiskAnalyzer sınıfı. Belirtilen risk analizi ayarlarına dayalı bir Monte Carlo simülasyonu gerçekleştirir"
type: docs
weight: 1890
url: /tr/net/aspose.tasks.riskanalysis/riskanalyzer/
---
## RiskAnalyzer class

Belirtilen risk analizi ayarlarına dayalı bir Monte Carlo simülasyonu gerçekleştirir.

```csharp
public class RiskAnalyzer
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [RiskAnalyzer](riskanalyzer/)(RiskAnalysisSettings) | `RiskAnalyzer` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Settings](../../aspose.tasks.riskanalysis/riskanalyzer/settings/) { get; set; } | Risk analizi için gerekli ayarları tanımlayan [`RiskAnalysisSettings`](../riskanalysissettings/) sınıfının örneğini alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Analyze](../../aspose.tasks.riskanalysis/riskanalyzer/analyze/)(Project) | Belirtilen proje için risk analizi gerçekleştirir. Analiz Monte Carlo simülasyonuna dayanır ve sonuç, [`RiskAnalysisResult`](../riskanalysisresult/) sınıfının bir örneğidir. |

## Örnekler

Risk analizine nasıl başlanacağını &lt;see cref="Aspose.Tasks.RiskAnalysis.RiskAnalysisSettings" /&gt; kullanarak gösterir.

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
var earlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", earlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", earlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", earlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", earlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", earlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", earlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", earlyFinish.Maximum);

settings = new RiskAnalysisSettings
{
    IterationsCount = 300
};

// ayarları değiştir
analyzer.Settings = settings;

analysisResult = analyzer.Analyze(project);
earlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

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


