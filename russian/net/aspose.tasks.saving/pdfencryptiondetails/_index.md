---
title: "Класс PdfEncryptionDetails"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Saving.PdfEncryptionDetails. Содержит детали для шифрования PDF"
type: docs
weight: 2110
url: /ru/net/aspose.tasks.saving/pdfencryptiondetails/
---
## PdfEncryptionDetails class

Содержит детали шифрования PDF.

```csharp
public class PdfEncryptionDetails
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PdfEncryptionDetails](pdfencryptiondetails/)(string, string, PdfEncryptionAlgorithm) | Инициализирует новый экземпляр класса `PdfEncryptionDetails`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [EncryptionAlgorithm](../../aspose.tasks.saving/pdfencryptiondetails/encryptionalgorithm/) { get; set; } | Получает или задает режим шифрования. |
| [OwnerPassword](../../aspose.tasks.saving/pdfencryptiondetails/ownerpassword/) { get; set; } | Получает или задает пароль владельца. |
| [Permissions](../../aspose.tasks.saving/pdfencryptiondetails/permissions/) { get; set; } | Получает или задает разрешения. |
| [UserPassword](../../aspose.tasks.saving/pdfencryptiondetails/userpassword/) { get; set; } | Получает или задает пароль пользователя. |

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


