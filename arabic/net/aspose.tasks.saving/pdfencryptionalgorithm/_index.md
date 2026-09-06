---
title: "التعداد PdfEncryptionAlgorithm"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.Saving.PdfEncryptionAlgorithm. يحدد خوارزمية التشفير المستخدمة لتشفير مستند PDF"
type: docs
weight: 2100
url: /ar/net/aspose.tasks.saving/pdfencryptionalgorithm/
---
## PdfEncryptionAlgorithm enumeration

يحدد خوارزمية التشفير المستخدمة لتشفير مستند PDF.

```csharp
public enum PdfEncryptionAlgorithm
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| RC4_40 | `0` | يحدد خوارزمية التشفير المستخدمة لتشفير مستند PDF. |
| RC4_128 | `1` | يحدد خوارزمية التشفير المستخدمة لتشفير مستند PDF. |

## الأمثلة

يظهر كيفية تحديد تفاصيل تشفير PDF أثناء حفظ المشروع كملف PDF

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// دعنا نحدد تفاصيل التشفير
var encryptionDetails = new PdfEncryptionDetails(
    // حدد كلمة مرور المستخدم
    "userPassword", 
    // حدد كلمة مرور المالك
    "ownerPassword", 
    // حدد خوارزمية التشفير
    PdfEncryptionAlgorithm.RC4_128);

// حدد الأذونات
encryptionDetails.Permissions = PdfPermissions.ModifyContents | PdfPermissions.ModifyAnnotations;

// اعرض كلمات مرور المستخدم والمالك
Console.WriteLine("User Password: " + encryptionDetails.UserPassword);
Console.WriteLine("Owner Password: " + encryptionDetails.OwnerPassword);
// اعرض وضع التشفير: RC4_40 أو RC4_128
Console.WriteLine("Encryption Algorithm: " + encryptionDetails.EncryptionAlgorithm);
Console.WriteLine("Permissions: " + encryptionDetails.Permissions);

var options = new PdfSaveOptions
{
    EncryptionDetails = encryptionDetails
};

// احفظ المشروع مع تفاصيل التشفير المحددة
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### انظر أيضًا

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


