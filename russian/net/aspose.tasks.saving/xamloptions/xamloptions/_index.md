---
title: "XamlOptions.XamlOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор XamlOptions. Инициализирует новый экземпляр класса XamlOptions, который может использоваться для сохранения проекта в формате XAML"
type: docs
weight: 10
url: /ru/net/aspose.tasks.saving/xamloptions/xamloptions/
---
## XamlOptions constructor

Инициализирует новый экземпляр класса [`XamlOptions`](../), который может использоваться для сохранения проекта в формате XAML.

```csharp
public XamlOptions()
```

## Примеры

Показывает, как сохранить проект в формате XAML, используя параметры сохранения.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new XamlOptions();
options.FitContent = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "RenderXAMLWithOptions_out.xaml", options);
```

### См. также

* class [XamlOptions](../)
* namespace [Aspose.Tasks.Saving](../../xamloptions/)
* assembly [Aspose.Tasks](../../../)


