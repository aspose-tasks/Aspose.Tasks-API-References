---
title: "PdfEncryptionDetails.Permissions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PdfEncryptionDetails. Получает или задает разрешения"
type: docs
weight: 40
url: /ru/net/aspose.tasks.saving/pdfencryptiondetails/permissions/
---
## PdfEncryptionDetails.Permissions property

Получает или задает разрешения.

```csharp
public PdfPermissions Permissions { get; set; }
```

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

* enum [PdfPermissions](../../pdfpermissions/)
* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


