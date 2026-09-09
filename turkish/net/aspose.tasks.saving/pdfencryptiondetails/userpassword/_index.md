---
title: "PdfEncryptionDetails.UserPassword"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PdfEncryptionDetails özelliği. Kullanıcı parolasını alır veya ayarlar."
type: docs
weight: 50
url: /tr/net/aspose.tasks.saving/pdfencryptiondetails/userpassword/
---
## PdfEncryptionDetails.UserPassword property

User parolasını alır veya ayarlar.

```csharp
public string UserPassword { get; set; }
```

## Açıklamalar

Belgeyi doğru kullanıcı parolasıyla (veya kullanıcı parolası olmayan bir belgeyi) açmak, belgenin şifreleme sözlüğünde belirtilen kullanıcı erişim izinlerine göre ek işlemlerin yapılmasına izin verir.

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

* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


