---
title: "PdfSaveOptions.EncryptionDetails"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PdfSaveOptions. Получает или задает детали шифрования. Если не задано, шифрование не будет выполнено."
type: docs
weight: 40
url: /ru/net/aspose.tasks.saving/pdfsaveoptions/encryptiondetails/
---
## PdfSaveOptions.EncryptionDetails property

Получает или задает детали шифрования. Если не задано, шифрование не будет выполнено.

```csharp
public PdfEncryptionDetails EncryptionDetails { get; set; }
```

## Примеры

Показывает, как задать детали шифрования PDF‑документа. Если не задано, шифрование не будет выполнено.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var encryptionDetails = new PdfEncryptionDetails("userPassword", "ownerPassword", PdfEncryptionAlgorithm.RC4_128);

var options = new PdfSaveOptions();

// Задать детали шифрования PDF‑документа.
options.EncryptionDetails = encryptionDetails;

// настроить дополнительные свойства
// установить <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" />, в котором будет сохранён документ.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithEncryptionDetails_out.pdf", options);
```

### См. также

* class [PdfEncryptionDetails](../../pdfencryptiondetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


