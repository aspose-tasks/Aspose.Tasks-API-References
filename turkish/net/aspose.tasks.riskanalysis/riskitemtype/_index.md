---
title: "Enum RiskItemType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.RiskAnalysis.RiskItemType enum. Risk analizi sırasında istatistiksel bilginin toplandığı görev alanlarını belirtir"
type: docs
weight: 1920
url: /tr/net/aspose.tasks.riskanalysis/riskitemtype/
---
## RiskItemType enumeration

Risk analizi sırasında istatistiksel bilginin toplandığı görev alanlarını belirtir.

```csharp
public enum RiskItemType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Start | `0` | Görev Başlangıcı. |
| Finish | `1` | Görev Bitişi. |
| EarlyStart | `2` | Görev Erken Başlangıç. |
| EarlyFinish | `3` | Görev Erken Bitiş. |
| LateStart | `4` | Görev Geç Başlangıç. |
| LateFinish | `5` | Görev Geç Bitiş. |

## Örnekler

Risk istatistiklerini nasıl hesaplayacağınızı ve PDF raporu olarak nasıl kaydedeceğinizi gösterir.

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

// analizi dosya yoluyla bir dosyaya rapor olarak kaydet
analysisResult.SaveReport(OutDir + "AnalysisResult_out.pdf");

// veya analizi bir akışa kaydet
using (var stream = new FileStream(OutDir + "AnalysisResult_out1.pdf", FileMode.Create))
{
    analysisResult.SaveReport(stream);
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


