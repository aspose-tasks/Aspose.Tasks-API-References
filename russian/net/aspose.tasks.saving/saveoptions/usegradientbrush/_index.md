---
title: "SaveOptions.UseGradientBrush"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SaveOptions. Получает или задает значение, указывающее, следует ли использовать градиентную кисть при рендеринге диаграммы Ганта"
type: docs
weight: 220
url: /ru/net/aspose.tasks.saving/saveoptions/usegradientbrush/
---
## SaveOptions.UseGradientBrush property

Получает или задает значение, указывающее, следует ли использовать градиентную кисть при рендеринге диаграммы Ганта.

```csharp
public virtual bool UseGradientBrush { get; set; }
```

## Примечания

Применяется только при рендеринге представления диаграммы Ганта.

## Примеры

показывает, как установить значение, указывающее, следует ли использовать градиентную кисть при рендеринге диаграммы Ганта.

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

### См. также

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


