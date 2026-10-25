---
title: "PdfEncryptionDetails.PdfEncryptionDetails"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PdfEncryptionDetails yapıcı. PdfEncryptionDetails sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks.saving/pdfencryptiondetails/pdfencryptiondetails/
---
## PdfEncryptionDetails constructor

[`PdfEncryptionDetails`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public PdfEncryptionDetails(string userPassword, string ownerPassword, 
    PdfEncryptionAlgorithm encryptionAlgorithm)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| userPassword | Dize | Korunan belgeleri açmaya izin veren kullanıcı parolası. |
| ownerPassword | Dize | Korunan belgeleri açmaya izin veren sahibi parolası. |
| encryptionAlgorithm | PdfEncryptionAlgorithm | Şifreleme algoritmasını belirten [`PdfEncryptionAlgorithm`](../../pdfencryptionalgorithm/) örneği. |

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

* enum [PdfEncryptionAlgorithm](../../pdfencryptionalgorithm/)
* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


