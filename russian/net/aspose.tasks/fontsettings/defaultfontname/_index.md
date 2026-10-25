---
title: "FontSettings.DefaultFontName"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство FontSettings. Получает или задает шрифт по умолчанию или резервный шрифт для рендеринга"
type: docs
weight: 20
url: /ru/net/aspose.tasks/fontsettings/defaultfontname/
---
## FontSettings.DefaultFontName property

Получает или задает шрифт по умолчанию (или резервный) для рендеринга.

```csharp
public string DefaultFontName { get; set; }
```

## Примеры

Показывает, как установить пользовательский шрифт, который будет использоваться при печати выходного PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart, FitContent = true
                  };

options.FontSettings.UseProjectDefaultFont = false;
options.FontSettings.DefaultFontName = "Segoe UI Black";
project.Save(OutDir + "CreateProject2_out.pdf", options);
```

### См. также

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


