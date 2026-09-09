---
title: "Enum Timescale"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.Timescale enum. Proje bir grafik formatına dışa aktarıldığında Gantt Şeması Görev Kullanımı veya Kaynak Kullanımı görünümlerinde zaman ölçeğinin nasıl render edileceğini belirten seçenekleri tanımlar."
type: docs
weight: 3430
url: /tr/net/aspose.tasks.visualization/timescale/
---
## Timescale enumeration

Proje grafik formatına dışa aktarıldığında Gantt Şeması, Görev Kullanımı veya Kaynak Kullanımı görünümlerinde zaman ölçeğinin nasıl render edileceğini belirten seçenekleri tanımlar.

```csharp
public enum Timescale
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| DefinedInView | `0` | Proje görünümünün özelliklerinde tanımlanan zaman ölçeği ayarlarını kullanın: [`BottomTimescaleTier`](../../aspose.tasks/ganttchartview/bottomtimescaletier/), [`MiddleTimescaleTier`](../../aspose.tasks/ganttchartview/middletimescaletier/), [`TopTimescaleTier`](../../aspose.tasks/ganttchartview/toptimescaletier/). Görünüm verisi içeren formatlar için geçerlidir. Örneğin, MPP formatından okunan projeler. |
| Days | `1` | Minimum detay seviyesinin bir gün olduğu önceden tanımlı iki katmanlı zaman ölçeği. |
| ThirdsOfMonths | `10` | Detay seviyesinin ayın üçte biri olduğu önceden tanımlı iki katmanlı zaman ölçeği. |
| Months | `30` | Minimum detay seviyesinin bir ay olduğu önceden tanımlı iki katmanlı zaman ölçeği. |

## Örnekler

Projenin SVG dosyası olarak nasıl kaydedileceğini gösterir.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
SaveOptions options = new SvgOptions
                        {
                            // belgenin kaydedileceği <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" />'ı ayarlayın
                            PresentationFormat = PresentationFormat.GanttChart,

                            // Satır yüksekliğinin içeriğe sığacak şekilde artırılıp artırılmayacağını gösteren bir değeri ayarlayın
                            FitContent = true,

                            // Render için minimum zaman periyodunu ayarlayın. Varsayılan değer <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.Timescale\">Days</see>'dir
                            Timescale = Timescale.ThirdsOfMonths,

                            // Proje düzenini render ederken gradyan fırça kullanılıp kullanılmayacağını belirler
                            // Şu anda gradyan fırçanın SVG'ye render edilmesi desteklenmemektedir.
                            // UseGradientBrush = true
                        };
project.Save(OutDir + "UseSvgOptions_out.svg", options);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


