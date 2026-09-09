---
title: "SaveOptions.UseGradientBrush"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveOptions özelliği. Gantt Şeması render edilirken degrade fırçasının kullanılıp kullanılmayacağını belirten bir değeri alır veya ayarlar"
type: docs
weight: 220
url: /tr/net/aspose.tasks.saving/saveoptions/usegradientbrush/
---
## SaveOptions.UseGradientBrush property

Gantt Şeması render edilirken degrade fırçasının kullanılıp kullanılmayacağını belirten bir değeri alır veya ayarlar.

```csharp
public virtual bool UseGradientBrush { get; set; }
```

## Açıklamalar

Yalnızca Gantt şeması görünümü render edildiğinde uygulanır.

## Örnekler

Gantt Şeması render edilirken degrade fırçasının kullanılıp kullanılmayacağını belirten bir değerin nasıl ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

SaveOptions options = new XamlOptions
{
    UseGradientBrush = false
};
project.Save(OutDir + "ChangeGanttBarsColorGradient_Solid_out.xaml", options);

options.UseGradientBrush = true;
project.Save(OutDir + "ChangeGanttBarsColorGradient_Gradient_out.xaml", options);
```

### Ayrıca Bakınız

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


