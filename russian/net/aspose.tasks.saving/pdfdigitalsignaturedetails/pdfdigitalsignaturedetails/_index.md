---
title: "PdfDigitalSignatureDetails.PdfDigitalSignatureDetails"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор PdfDigitalSignatureDetails. Инициализирует новый экземпляр класса PdfDigitalSignatureDetails"
type: docs
weight: 10
url: /ru/net/aspose.tasks.saving/pdfdigitalsignaturedetails/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails constructor

Инициализирует новый экземпляр класса [`PdfDigitalSignatureDetails`](../).

```csharp
public PdfDigitalSignatureDetails(X509Certificate2 certificate, string reason, string location, 
    DateTime signatureDate, PdfDigitalSignatureHashAlgorithm hashAlgorithm)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| сертификат | X509Certificate2 | Экземпляр X509Certificate2, которым будет выполнена подпись. |
| причина | Строка | Причина подписания. |
| место | Строка | Место подписания. |
| signatureDate | DateTime | Дата подписания. |
| hashAlgorithm | PdfDigitalSignatureHashAlgorithm | Алгоритм хеширования подписи. |

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

* enum [PdfDigitalSignatureHashAlgorithm](../../pdfdigitalsignaturehashalgorithm/)
* class [PdfDigitalSignatureDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfdigitalsignaturedetails/)
* assembly [Aspose.Tasks](../../../)


