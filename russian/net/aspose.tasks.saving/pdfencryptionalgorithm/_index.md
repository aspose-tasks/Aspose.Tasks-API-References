---
title: "Перечисление PdfEncryptionAlgorithm"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.Saving.PdfEncryptionAlgorithm. Указывает алгоритм шифрования, используемый для шифрования PDF‑документа"
type: docs
weight: 2100
url: /ru/net/aspose.tasks.saving/pdfencryptionalgorithm/
---
## PdfEncryptionAlgorithm enumeration

Указывает алгоритм шифрования, используемый для шифрования PDF‑документа.

```csharp
public enum PdfEncryptionAlgorithm
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| RC4_40 | `0` | Указывает алгоритм шифрования, используемый для шифрования PDF‑документа. |
| RC4_128 | `1` | Указывает алгоритм шифрования, используемый для шифрования PDF‑документа. |

## Примеры

Показывает, как указать детали шифрования PDF при сохранении проекта в файл PDF.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// указываем детали шифрования
var encryptionDetails = new PdfEncryptionDetails(
    // указать пароль пользователя
    "userPassword", 
    // указать пароль владельца
    "ownerPassword", 
    // указать алгоритм шифрования
    PdfEncryptionAlgorithm.RC4_128);

// указать разрешения
encryptionDetails.Permissions = PdfPermissions.ModifyContents | PdfPermissions.ModifyAnnotations;

// показать пароли пользователя и владельца
Console.WriteLine("User Password: " + encryptionDetails.UserPassword);
Console.WriteLine("Owner Password: " + encryptionDetails.OwnerPassword);
// показать режим шифрования: RC4_40 или RC4_128
Console.WriteLine("Encryption Algorithm: " + encryptionDetails.EncryptionAlgorithm);
Console.WriteLine("Permissions: " + encryptionDetails.Permissions);

var options = new PdfSaveOptions
{
    EncryptionDetails = encryptionDetails
};

// сохранить проект с указанными деталями шифрования
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### См. также

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


