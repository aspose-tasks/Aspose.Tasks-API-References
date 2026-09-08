---
title: "HtmlSaveOptions.UseGradientBrush"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство HtmlSaveOptions. Получает или задает значение, указывающее, использовать ли градиентную кисть при рендеринге макета проекта. В настоящее время использование градиентной кисти не поддерживается при рендеринге в HTML."
type: docs
weight: 160
url: /ru/net/aspose.tasks.saving/htmlsaveoptions/usegradientbrush/
---
## HtmlSaveOptions.UseGradientBrush property

Получает или задает значение, указывающее, использовать ли градиентную кисть при отрисовке макета проекта. В настоящее время использование градиентной кисти не поддерживается при отрисовке в HTML.

```csharp
public override bool UseGradientBrush { get; set; }
```

## Примеры

Показывает, как задать пользовательский шрифт, который будет использоваться для экспорта проекта в HTML-файл.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart,
                      FitContent = true
                  };

options.FontSettings.UseProjectDefaultFont = false;
options.FontSettings.DefaultFontName = "Segoe UI Black";
project.Save(OutDir + "AddDefaultFontDuringSavingAsHtml_out.html", options);
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


