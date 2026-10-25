---
title: "XamlOptions.XamlOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "XamlOptions yapıcı. Projeyi XAML formatında kaydetmek için kullanılabilecek XamlOptions sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks.saving/xamloptions/xamloptions/
---
## XamlOptions constructor

Projeyi XAML formatında kaydetmek için kullanılabilecek [`XamlOptions`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public XamlOptions()
```

## Örnekler

Kaydetme seçeneklerini kullanarak bir projeyi XAML formatında nasıl kaydedeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new XamlOptions();
options.FitContent = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "RenderXAMLWithOptions_out.xaml", options);
```

### Ayrıca Bakınız

* class [XamlOptions](../)
* namespace [Aspose.Tasks.Saving](../../xamloptions/)
* assembly [Aspose.Tasks](../../../)


