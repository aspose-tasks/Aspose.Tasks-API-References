---
title: "PdfSaveOptions.Compliance"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PdfSaveOptions. Получает или задает требуемый уровень соответствия для генерируемого PDF‑документа. По умолчанию — Pdf15."
type: docs
weight: 20
url: /ru/net/aspose.tasks.saving/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

Получает или задает желаемый уровень соответствия для создаваемого PDF‑документа. По умолчанию — Pdf15.

```csharp
public PdfCompliance Compliance { get; set; }
```

## Примеры

Показывает, как установить желаемый уровень соответствия для генерируемого PDF‑документа.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// установить желаемый уровень соответствия для генерируемого PDF‑документа
// по умолчанию тип <see cref=\"PdfCompliance.Pdf15\"/>
options.Compliance = PdfCompliance.PdfA1b;

// настроить дополнительные свойства
// установить <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" />, в котором будет сохранён документ.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithPdfCompliance_out.pdf", options);
```

### См. также

* enum [PdfCompliance](../../pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


