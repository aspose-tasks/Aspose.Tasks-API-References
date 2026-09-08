---
title: "PdfEncryptionDetails.PdfEncryptionDetails"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор PdfEncryptionDetails. Инициализирует новый экземпляр класса PdfEncryptionDetails."
type: docs
weight: 10
url: /ru/net/aspose.tasks.saving/pdfencryptiondetails/pdfencryptiondetails/
---
## PdfEncryptionDetails constructor

Инициализирует новый экземпляр класса [`PdfEncryptionDetails`](../).

```csharp
public PdfEncryptionDetails(string userPassword, string ownerPassword, 
    PdfEncryptionAlgorithm encryptionAlgorithm)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| userPassword | Строка | Пароль пользователя, позволяющий открыть защищённые документы. |
| ownerPassword | Строка | Пароль владельца, позволяющий открыть защищённые документы. |
| encryptionAlgorithm | PdfEncryptionAlgorithm | Экземпляр [`PdfEncryptionAlgorithm`](../../pdfencryptionalgorithm/), указывающий алгоритм шифрования. |

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

* enum [PdfEncryptionAlgorithm](../../pdfencryptionalgorithm/)
* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


