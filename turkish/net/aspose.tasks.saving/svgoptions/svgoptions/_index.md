---
title: "SvgOptions.SvgOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SvgOptions yapıcı. Projeyi SVG formatında kaydetmek için kullanılabilecek SvgOptions sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks.saving/svgoptions/svgoptions/
---
## SvgOptions constructor

[`SvgOptions`](../) sınıfının yeni bir örneğini başlatır; bu, projeyi SVG formatında kaydetmekte kullanılabilir.

```csharp
public SvgOptions()
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


