---
title: "Enum ReportType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.ReportType enum. Projelerin grafik raporunun türü"
type: docs
weight: 3330
url: /tr/net/aspose.tasks.visualization/reporttype/
---
## ReportType enumeration

Projenin grafik raporunun türü.

```csharp
public enum ReportType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| ProjectOverview | `0` | Projenin başlangıç ve bitiş tarihlerini, sürenin tamamlanma yüzdesini, üst düzey görevlerin tamamlanma yüzdesini ve yaklaşan kilometre taşlarını gösterir. |
| CostOverview | `1` | Projenin başlangıç ve bitiş tarihlerini, mevcut planlanan ve kalan maliyeti, % Tamamlanma ve üst düzey görevlerin maliyet değerlerini gösterir. |
| WorkOverview | `2` | Her üst düzey görev için temel, gerçek ve kalan işi ve iş kaynakları için işi gösterir. |
| ResourceOverview | `3` | Kaynağa göre temel, gerçek ve kalan işi gösterir. |
| ResourceCostOverview | `4` | Kaynağa göre temel, gerçek ve kalan maliyeti gösterir. |
| CriticalTasks | `5` | Proje görevlerinden kritik olanları gösterir. |
| LateTasks | `6` | Geç kalan proje görevlerini gösterir. |
| Milestones | `7` | Geç kalan, yaklaşan ve tamamlanan kilometre taşlarını gösterir. |
| UpcomingTask | `8` | Mevcut hafta içinde teslim edilmesi gereken görevleri ve mevcut hafta içinde başlayan görevleri gösterir. |
| CostOverruns | `9` | Göreve ve kaynağa göre maliyet sapmasını gösterir. |
| TaskCostOverview | `10` | Tüm üst düzey görevlerin temel, gerçek ve kalan maliyetini gösterir. |
| OverallocatedResources | `11` | Aşırı tahsis edilmiş kaynaklar için kalan iş saatlerinin sayısını gösterir. |
| SlippingTasks | `12` | Temel bitiş tarihinden sonra bitmesi gereken görevleri gösterir (temel ayarlanmış olmalıdır). |
| BestPracticeAnalyzer | `13` | Gerçek işi olmayan, atanmamış görevleri, süresi 8 saatten az olan görevleri ve kaynaklarla atanan özetleri gösterir. |
| Burndown | `14` | İş burndown ve görev burndown grafiklerini içerir. İş burndown grafiği, insanların ne kadar işi tamamladığını, proje bitiş tarihinden önce ne kadarının planlandığını ve bu noktada projenin ne kadar işin tamamlanacağını gösteren temel tahminini gösterir. Görev burndown grafiği, tamamlanan görev sayısını, kalan görev sayısını ve bu noktada kaç görevin tamamlanacağını gösteren temel tahmini gösterir. |
| CashFlow | `15` | Tüm üst düzey görevler için çeyrek bazında maliyetleri ve birikimli maliyetleri gösterir. |

## Örnekler

Belirtilen akışa PDF formatında proje burndown raporunun nasıl kaydedileceğini gösterir.

```csharp
var project = new Project(DataDir + @"Homemoveplan.mpp");
using (var stream = new FileStream(OutDir + "Burndown_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


