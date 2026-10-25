---
title: "PdfEncryptionDetails.OwnerPassword"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PdfEncryptionDetails. تحصل أو تعين كلمة مرور المالك"
type: docs
weight: 30
url: /ar/net/aspose.tasks.saving/pdfencryptiondetails/ownerpassword/
---
## PdfEncryptionDetails.OwnerPassword property

يحصل أو يعيّن كلمة مرور المالك.

```csharp
public string OwnerPassword { get; set; }
```

## ملاحظات

فتح المستند باستخدام كلمة مرور المالك الصحيحة (مع افتراض أنها ليست هي نفسها كلمة مرور المستخدم) يتيح وصولًا كاملاً (كمالك) إلى المستند. هذا الوصول غير المحدود يشمل القدرة على تغيير كلمات مرور المستند وأذونات الوصول.

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

* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


