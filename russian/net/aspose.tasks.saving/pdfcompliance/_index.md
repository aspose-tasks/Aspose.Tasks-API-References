---
title: "Перечисление PdfCompliance"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.Saving.PdfCompliance. Указывает уровень соответствия PDF для выходного файла."
type: docs
weight: 2070
url: /ru/net/aspose.tasks.saving/pdfcompliance/
---
## PdfCompliance enumeration

Указывает уровень соответствия PDF для выходного файла.

```csharp
public enum PdfCompliance
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Pdf15 | `0` | Уровень соответствия PDF/15. |
| PdfA1a | `1` | Уровень соответствия PDF/A-1a. |
| PdfA1b | `2` | Уровень соответствия PDF/A-1b. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


