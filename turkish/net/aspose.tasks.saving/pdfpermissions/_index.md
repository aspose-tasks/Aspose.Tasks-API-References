---
title: "Enum PdfPermissions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Saving.PdfPermissions enum. PDF belgesine erişim için kullanılacak izinleri belirtir."
type: docs
weight: 2120
url: /tr/net/aspose.tasks.saving/pdfpermissions/
---
## PdfPermissions enumeration

Bir PDF belgesine erişmek için kullanılacak izinleri belirtir.

```csharp
public enum PdfPermissions
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Bir PDF belgesine erişmek için kullanılacak izinleri belirtir. |
| Printing | `4` | Bir PDF belgesine erişmek için kullanılacak izinleri belirtir. |
| ModifyContents | `8` | Bir PDF belgesine erişmek için kullanılacak izinleri belirtir. |
| ContentCopy | `16` | Bir PDF belgesine erişmek için kullanılacak izinleri belirtir. |
| ModifyAnnotations | `32` | Bir PDF belgesine erişmek için kullanılacak izinleri belirtir. |
| FillIn | `256` | Bir PDF belgesine erişmek için kullanılacak izinleri belirtir. |
| ContentCopyForAccessibility | `512` | Bir PDF belgesine erişmek için kullanılacak izinleri belirtir. |
| DocumentAssembly | `1024` | Bir PDF belgesine erişmek için kullanılacak izinleri belirtir. |
| HighResolutionPrinting | `2052` | Bir PDF belgesine erişmek için kullanılacak izinleri belirtir. |
| AllowAll | `65535` | Bir PDF belgesine erişmek için kullanılacak izinleri belirtir. |

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


