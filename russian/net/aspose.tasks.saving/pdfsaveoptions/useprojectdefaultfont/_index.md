---
title: "UseProjectDefaultFont"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Получает или задает значение, указывающее, должен ли использоваться шрифт по умолчанию для рендеринга."
type: docs
weight: 120
url: /ru/net/aspose.tasks.saving/pdfsaveoptions/useprojectdefaultfont/
---
## PdfSaveOptions.UseProjectDefaultFont property

Получает или задает значение, указывающее, должен ли использоваться шрифт по умолчанию для рендеринга.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

### Примечания

Если значение равно False и указано DefaultFontName, движок рендеринга будет использовать шрифт, указанный в DefaultFontName, в качестве резервного шрифта. В противном случае в качестве резервного шрифта используются 'Arial' (если установлен) или шрифты 'Generic Sans Serif'. Резервный шрифт используется при рендеринге представления проекта, когда стиль текста ссылается на шрифт, не установленный в текущей операционной системе. Для более тонкого управления разрешением шрифтов вы можете использовать обратный вызов [`FontResolveCallback`](../fontresolvecallback).

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
