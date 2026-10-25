---
title: "الفئة PdfEncryptionDetails"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Saving.PdfEncryptionDetails. تحتوي على تفاصيل لتشفير PDF"
type: docs
weight: 2110
url: /ar/net/aspose.tasks.saving/pdfencryptiondetails/
---
## PdfEncryptionDetails class

يحتوي على تفاصيل لتشفير PDF.

```csharp
public class PdfEncryptionDetails
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PdfEncryptionDetails](pdfencryptiondetails/)(string, string, PdfEncryptionAlgorithm) | يُنشئ مثلاً جديداً من الفئة `PdfEncryptionDetails`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [EncryptionAlgorithm](../../aspose.tasks.saving/pdfencryptiondetails/encryptionalgorithm/) { get; set; } | يحصل أو يعيّن وضع التشفير. |
| [OwnerPassword](../../aspose.tasks.saving/pdfencryptiondetails/ownerpassword/) { get; set; } | يحصل أو يعيّن كلمة مرور المالك. |
| [Permissions](../../aspose.tasks.saving/pdfencryptiondetails/permissions/) { get; set; } | يحصل أو يعيّن الأذونات. |
| [UserPassword](../../aspose.tasks.saving/pdfencryptiondetails/userpassword/) { get; set; } | يحصل أو يعيّن كلمة مرور المستخدم. |

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


