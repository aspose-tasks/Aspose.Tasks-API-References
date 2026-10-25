---
title: "PdfEncryptionDetails.PdfEncryptionDetails"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ PdfEncryptionDetails. يهيئ مثيلًا جديدًا من الفئة PdfEncryptionDetails"
type: docs
weight: 10
url: /ar/net/aspose.tasks.saving/pdfencryptiondetails/pdfencryptiondetails/
---
## PdfEncryptionDetails constructor

يهيئ مثيلًا جديدًا من الفئة [`PdfEncryptionDetails`](../).

```csharp
public PdfEncryptionDetails(string userPassword, string ownerPassword, 
    PdfEncryptionAlgorithm encryptionAlgorithm)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| userPassword | سلسلة | كلمة مرور المستخدم التي تسمح بفتح المستندات المحمية. |
| ownerPassword | سلسلة | كلمة مرور المالك التي تسمح بفتح المستندات المحمية. |
| encryptionAlgorithm | PdfEncryptionAlgorithm | مثيل [`PdfEncryptionAlgorithm`](../../pdfencryptionalgorithm/) الذي يشير إلى خوارزمية التشفير. |

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

* enum [PdfEncryptionAlgorithm](../../pdfencryptionalgorithm/)
* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


