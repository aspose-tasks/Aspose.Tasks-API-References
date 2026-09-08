---
title: "DefaultFontName"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Получает или задает шрифт по умолчанию или резервный шрифт для рендеринга."
type: docs
weight: 40
url: /ru/net/aspose.tasks.saving/htmlsaveoptions/defaultfontname/
---
## HtmlSaveOptions.DefaultFontName property

Получает или задает шрифт по умолчанию (или резервный) для рендеринга.

```csharp
public string DefaultFontName { get; set; }
```

### Примеры

Показывает, как задать пользовательский шрифт, который будет использоваться для экспорта проекта в HTML-файл.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart,
                      FitContent = true,
                      UseProjectDefaultFont = false,
                      DefaultFontName = "Segoe UI Black"
                  };
project.Save(OutDir + "AddDefaultFontDuringSavingAsHtml_out.html", options);
```

### См. также

* class [HtmlSaveOptions](../../htmlsaveoptions)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для Aspose.Tasks.dll -->
