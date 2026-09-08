---
title: "Перечисление PdfTextCompression"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Saving.PdfTextCompression перечисление. Указывает тип сжатия, применяемого ко всему содержимому PDF‑файла, кроме изображений."
type: docs
weight: 2140
url: /ru/net/aspose.tasks.saving/pdftextcompression/
---
## PdfTextCompression enumeration

Указывает тип сжатия, применяемый ко всему содержимому PDF‑файла, кроме изображений.

```csharp
public enum PdfTextCompression
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Без сжатия. |
| Flate | `1` | Сжатие Flate. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


