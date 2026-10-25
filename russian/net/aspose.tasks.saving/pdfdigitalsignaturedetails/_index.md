---
title: "Класс PdfDigitalSignatureDetails"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Saving.PdfDigitalSignatureDetails. Содержит детали цифровой подписи PDF."
type: docs
weight: 2080
url: /ru/net/aspose.tasks.saving/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails class

Содержит детали цифровой подписи PDF.

```csharp
public class PdfDigitalSignatureDetails
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PdfDigitalSignatureDetails](pdfdigitalsignaturedetails/)(X509Certificate2, string, string, DateTime, PdfDigitalSignatureHashAlgorithm) | Инициализирует новый экземпляр класса `PdfDigitalSignatureDetails`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Certificate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/certificate/) { get; set; } | Получает или задает сертификат для подписи. |
| [HashAlgorithm](../../aspose.tasks.saving/pdfdigitalsignaturedetails/hashalgorithm/) { get; set; } | Получает или задает алгоритм хеширования. |
| [Location](../../aspose.tasks.saving/pdfdigitalsignaturedetails/location/) { get; set; } | Получает или задает место подписи. |
| [Reason](../../aspose.tasks.saving/pdfdigitalsignaturedetails/reason/) { get; set; } | Получает или задает причину подписи. |
| [SignatureDate](../../aspose.tasks.saving/pdfdigitalsignaturedetails/signaturedate/) { get; set; } | Получает или задает дату подписи. |

## Примечания

В данный момент цифровая подпись PDF‑документов доступна только в .NET 2.0 и выше.

## Примеры

Показывает, как работать с деталями цифровой подписи PDF.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new PdfSaveOptions();

var certificate = new X509Certificate2();

// создать детали подписи PDF
var signatureDetails = new PdfDigitalSignatureDetails(
    // указать сертификат
    certificate, 
    // указать причину подписи
    "reason",
    // указать место подписи
    "location", 
    // указать дату подписи
    new DateTime(2019, 1, 1), 
    // указать хеш‑алгоритм подписи
    PdfDigitalSignatureHashAlgorithm.Sha1);

Console.WriteLine("Certificate: " + signatureDetails.Certificate);
Console.WriteLine("Reason: " + signatureDetails.Reason);
Console.WriteLine("Location: " + signatureDetails.Location);
Console.WriteLine("Signature Date: " + signatureDetails.SignatureDate);
Console.WriteLine("Hash Algorithm: " + signatureDetails.HashAlgorithm);

// установить детали цифровой подписи
options.DigitalSignatureDetails = signatureDetails;

// сохранить проект с указанными деталями шифрования
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### См. также

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


