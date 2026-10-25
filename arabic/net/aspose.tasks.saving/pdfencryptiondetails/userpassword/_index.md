---
title: "PdfEncryptionDetails.UserPassword"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PdfEncryptionDetails. تحصل أو تعين كلمة مرور المستخدم"
type: docs
weight: 50
url: /ar/net/aspose.tasks.saving/pdfencryptiondetails/userpassword/
---
## PdfEncryptionDetails.UserPassword property

يحصل أو يعيّن كلمة مرور المستخدم.

```csharp
public string UserPassword { get; set; }
```

## ملاحظات

فتح المستند باستخدام كلمة مرور المستخدم الصحيحة (أو فتح مستند لا يحتوي على كلمة مرور مستخدم) يتيح تنفيذ عمليات إضافية وفقًا لأذونات الوصول للمستخدم المحددة في قاموس تشفير المستند.

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


