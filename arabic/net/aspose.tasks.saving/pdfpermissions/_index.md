---
title: "تعداد PdfPermissions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.Saving.PdfPermissions. يحدد الأذونات المستخدمة للوصول إلى مستند PDF."
type: docs
weight: 2120
url: /ar/net/aspose.tasks.saving/pdfpermissions/
---
## PdfPermissions enumeration

يحدد الأذونات المستخدمة للوصول إلى مستند PDF.

```csharp
public enum PdfPermissions
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | يحدد الأذونات المستخدمة للوصول إلى مستند PDF. |
| Printing | `4` | يحدد الأذونات المستخدمة للوصول إلى مستند PDF. |
| ModifyContents | `8` | يحدد الأذونات المستخدمة للوصول إلى مستند PDF. |
| ContentCopy | `16` | يحدد الأذونات المستخدمة للوصول إلى مستند PDF. |
| ModifyAnnotations | `32` | يحدد الأذونات المستخدمة للوصول إلى مستند PDF. |
| FillIn | `256` | يحدد الأذونات المستخدمة للوصول إلى مستند PDF. |
| ContentCopyForAccessibility | `512` | يحدد الأذونات المستخدمة للوصول إلى مستند PDF. |
| DocumentAssembly | `1024` | يحدد الأذونات المستخدمة للوصول إلى مستند PDF. |
| HighResolutionPrinting | `2052` | يحدد الأذونات المستخدمة للوصول إلى مستند PDF. |
| AllowAll | `65535` | يحدد الأذونات المستخدمة للوصول إلى مستند PDF. |

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


