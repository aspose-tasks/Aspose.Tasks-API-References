---
title: "Перечисление PdfPermissions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.Saving.PdfPermissions. Указывает разрешения, используемые для доступа к PDF‑документу."
type: docs
weight: 2120
url: /ru/net/aspose.tasks.saving/pdfpermissions/
---
## PdfPermissions enumeration

Указывает разрешения, используемые для доступа к PDF‑документу.

```csharp
public enum PdfPermissions
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Указывает разрешения, используемые для доступа к PDF‑документу. |
| Printing | `4` | Указывает разрешения, используемые для доступа к PDF‑документу. |
| ModifyContents | `8` | Указывает разрешения, используемые для доступа к PDF‑документу. |
| ContentCopy | `16` | Указывает разрешения, используемые для доступа к PDF‑документу. |
| ModifyAnnotations | `32` | Указывает разрешения, используемые для доступа к PDF‑документу. |
| FillIn | `256` | Указывает разрешения, используемые для доступа к PDF‑документу. |
| ContentCopyForAccessibility | `512` | Указывает разрешения, используемые для доступа к PDF‑документу. |
| DocumentAssembly | `1024` | Указывает разрешения, используемые для доступа к PDF‑документу. |
| HighResolutionPrinting | `2052` | Указывает разрешения, используемые для доступа к PDF‑документу. |
| AllowAll | `65535` | Указывает разрешения, используемые для доступа к PDF‑документу. |

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


