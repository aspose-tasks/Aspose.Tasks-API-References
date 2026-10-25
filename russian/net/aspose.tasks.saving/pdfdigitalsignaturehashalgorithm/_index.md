---
title: "Enum PdfDigitalSignatureHashAlgorithm"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Saving.PdfDigitalSignatureHashAlgorithm enum. Указывает цифровой хеш‑алгоритм, используемый цифровой подписью."
type: docs
weight: 2090
url: /ru/net/aspose.tasks.saving/pdfdigitalsignaturehashalgorithm/
---
## PdfDigitalSignatureHashAlgorithm enumeration

Указывает алгоритм цифрового хеша, используемый цифровой подписью.

```csharp
public enum PdfDigitalSignatureHashAlgorithm
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Sha1 | `0` | Указывает цифровой хеш‑алгоритм, используемый цифровой подписью. |
| Sha256 | `1` | Указывает цифровой хеш‑алгоритм, используемый цифровой подписью. |
| Sha384 | `2` | Указывает цифровой хеш‑алгоритм, используемый цифровой подписью. |
| Sha512 | `3` | Указывает цифровой хеш‑алгоритм, используемый цифровой подписью. |
| Md5 | `4` | Указывает цифровой хеш‑алгоритм, используемый цифровой подписью. |

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


