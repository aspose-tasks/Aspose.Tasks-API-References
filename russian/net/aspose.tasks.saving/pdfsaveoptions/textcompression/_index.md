---
title: "PdfSaveOptions.TextCompression"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PdfSaveOptions. Получает или задает тип сжатия, используемый для всех потоков содержимого, кроме изображений. По умолчанию — Flate."
type: docs
weight: 100
url: /ru/net/aspose.tasks.saving/pdfsaveoptions/textcompression/
---
## PdfSaveOptions.TextCompression property

Получает или задает тип сжатия, используемый для всех потоков содержимого, кроме изображений. По умолчанию — Flate.

```csharp
public PdfTextCompression TextCompression { get; set; }
```

## Примеры

Показывает, как установить тип сжатия, используемый для всех потоков содержимого, кроме изображений.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// установить тип сжатия, используемый для всех потоков содержимого, кроме изображений
options.TextCompression = PdfTextCompression.Flate;

// настроить дополнительные свойства
// установить <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" />, в котором будет сохранён документ.
options.PresentationFormat = PresentationFormat.GanttChart;

// установить желаемый уровень соответствия для генерируемого PDF‑документа
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithTextCompression_out.pdf", options);
```

### См. также

* enum [PdfTextCompression](../../pdftextcompression/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


