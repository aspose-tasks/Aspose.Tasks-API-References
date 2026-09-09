---
title: "SvgOptions.UseGradientBrush"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SvgOptions özelliği. Proje düzeni render edilirken degrade fırçası kullanılıp kullanılmayacağını belirler. Şu anda SVG'ye render ederken degrade fırçası kullanımı desteklenmemektedir."
type: docs
weight: 30
url: /tr/net/aspose.tasks.saving/svgoptions/usegradientbrush/
---
## SvgOptions.UseGradientBrush property

Proje düzenini render ederken gradyan fırça kullanılıp kullanılmayacağını belirler. Şu anda gradyan fırçanın SVG'ye render edilmesi desteklenmemektedir.

```csharp
public override bool UseGradientBrush { get; set; }
```

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

* class [SvgOptions](../)
* namespace [Aspose.Tasks.Saving](../../svgoptions/)
* assembly [Aspose.Tasks](../../../)


