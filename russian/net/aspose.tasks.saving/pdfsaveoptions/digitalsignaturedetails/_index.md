---
title: "PdfSaveOptions.DigitalSignatureDetails"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PdfSaveOptions. Получает или задает детали цифровой подписи. Если не задано, подпись не будет выполнена."
type: docs
weight: 30
url: /ru/net/aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/
---
## PdfSaveOptions.DigitalSignatureDetails property

Получает или задает детали цифровой подписи. Если не задано, подпись не будет выполнена.

```csharp
public PdfDigitalSignatureDetails DigitalSignatureDetails { get; set; }
```

## Примеры

Показывает, как задать детали цифровой подписи. Если не задано, подпись не будет выполнена.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
var certificate = new X509Certificate2();

// Задать детали цифровой подписи. Если не задано, подпись не будет выполнена.
options.DigitalSignatureDetails = new PdfDigitalSignatureDetails(
    certificate,
    "reason",
    "location",
    new DateTime(2019, 1, 1),
    PdfDigitalSignatureHashAlgorithm.Sha1);

// настроить дополнительные свойства
// установить <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" />, в котором будет сохранён документ.
options.PresentationFormat = PresentationFormat.GanttChart;

// установить желаемый уровень соответствия для генерируемого PDF‑документа
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithDigitalSignatureDetails_out.pdf", options);
```

### См. также

* class [PdfDigitalSignatureDetails](../../pdfdigitalsignaturedetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


