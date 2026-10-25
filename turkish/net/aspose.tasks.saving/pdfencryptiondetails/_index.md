---
title: "Sınıf PdfEncryptionDetails"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Saving.PdfEncryptionDetails sınıfı. PDF şifrelemesi için ayrıntıları içerir"
type: docs
weight: 2110
url: /tr/net/aspose.tasks.saving/pdfencryptiondetails/
---
## PdfEncryptionDetails class

PDF şifrelemesi için ayrıntılar içerir.

```csharp
public class PdfEncryptionDetails
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PdfEncryptionDetails](pdfencryptiondetails/)(string, string, PdfEncryptionAlgorithm) | `PdfEncryptionDetails` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [EncryptionAlgorithm](../../aspose.tasks.saving/pdfencryptiondetails/encryptionalgorithm/) { get; set; } | Şifreleme modunu alır veya ayarlar. |
| [OwnerPassword](../../aspose.tasks.saving/pdfencryptiondetails/ownerpassword/) { get; set; } | Owner parolasını alır veya ayarlar. |
| [Permissions](../../aspose.tasks.saving/pdfencryptiondetails/permissions/) { get; set; } | İzinleri alır veya ayarlar. |
| [UserPassword](../../aspose.tasks.saving/pdfencryptiondetails/userpassword/) { get; set; } | User parolasını alır veya ayarlar. |

## Örnekler

Bir projeyi PDF dosyası olarak kaydederken PDF şifreleme ayrıntılarını nasıl belirteceğinizi gösterir.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// şifreleme ayrıntılarını belirleyelim
var encryptionDetails = new PdfEncryptionDetails(
    // kullanıcı parolasını belirle
    "userPassword", 
    // sahip parolasını belirle
    "ownerPassword", 
    // şifreleme algoritmasını belirle
    PdfEncryptionAlgorithm.RC4_128);

// izinleri belirle
encryptionDetails.Permissions = PdfPermissions.ModifyContents | PdfPermissions.ModifyAnnotations;

// kullanıcı ve sahip parolalarını göster
Console.WriteLine("User Password: " + encryptionDetails.UserPassword);
Console.WriteLine("Owner Password: " + encryptionDetails.OwnerPassword);
// şifreleme modunu göster: RC4_40 veya RC4_128
Console.WriteLine("Encryption Algorithm: " + encryptionDetails.EncryptionAlgorithm);
Console.WriteLine("Permissions: " + encryptionDetails.Permissions);

var options = new PdfSaveOptions
{
    EncryptionDetails = encryptionDetails
};

// belirtilen şifreleme ayrıntılarıyla projeyi kaydet
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


