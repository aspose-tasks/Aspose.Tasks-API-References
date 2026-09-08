---
title: "DefaultFontName"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Получает или задает шрифт по умолчанию или резервный шрифт для рендеринга."
type: docs
weight: 30
url: /ru/net/aspose.tasks.saving/pdfsaveoptions/defaultfontname/
---
## PdfSaveOptions.DefaultFontName property

Получает или задает шрифт по умолчанию (или резервный) для рендеринга.

```csharp
public string DefaultFontName { get; set; }
```

### Примеры

Показывает, как установить пользовательский шрифт, который будет использоваться при печати выходного PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart, FitContent = true, UseProjectDefaultFont = false, DefaultFontName = "Segoe UI Black"
                  };
project.Save(OutDir + "CreateProject2_out.pdf", options);
```

### См. также

* class [PdfSaveOptions](../../pdfsaveoptions)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для Aspose.Tasks.dll -->
