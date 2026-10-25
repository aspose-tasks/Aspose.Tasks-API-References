---
title: "क्लास PdfEncryptionDetails"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Saving.PdfEncryptionDetails क्लास। PDF एन्क्रिप्शन के विवरण शामिल करता है"
type: docs
weight: 2110
url: /hi/net/aspose.tasks.saving/pdfencryptiondetails/
---
## PdfEncryptionDetails class

PDF एन्क्रिप्शन के विवरण शामिल करता है।

```csharp
public class PdfEncryptionDetails
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [PdfEncryptionDetails](pdfencryptiondetails/)(string, string, PdfEncryptionAlgorithm) | `PdfEncryptionDetails` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [EncryptionAlgorithm](../../aspose.tasks.saving/pdfencryptiondetails/encryptionalgorithm/) { get; set; } | एन्क्रिप्शन मोड को प्राप्त करता है या सेट करता है। |
| [OwnerPassword](../../aspose.tasks.saving/pdfencryptiondetails/ownerpassword/) { get; set; } | ओनर पासवर्ड को प्राप्त करता है या सेट करता है। |
| [Permissions](../../aspose.tasks.saving/pdfencryptiondetails/permissions/) { get; set; } | अनुमतियों को प्राप्त करता है या सेट करता है। |
| [UserPassword](../../aspose.tasks.saving/pdfencryptiondetails/userpassword/) { get; set; } | यूज़र पासवर्ड को प्राप्त करता है या सेट करता है। |

## उदाहरण

प्रोजेक्ट को PDF फ़ाइल के रूप में सहेजते समय PDF एन्क्रिप्शन विवरण निर्दिष्ट करने के उपयोग को दिखाता है।

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// एन्क्रिप्शन विवरण निर्दिष्ट करें
var encryptionDetails = new PdfEncryptionDetails(
    // यूज़र पासवर्ड निर्दिष्ट करें
    "userPassword", 
    // ओनर पासवर्ड निर्दिष्ट करें
    "ownerPassword", 
    // एन्क्रिप्शन एल्गोरिदम निर्दिष्ट करें
    PdfEncryptionAlgorithm.RC4_128);

// अनुमतियों को निर्दिष्ट करें
encryptionDetails.Permissions = PdfPermissions.ModifyContents | PdfPermissions.ModifyAnnotations;

// यूज़र और ओनर पासवर्ड दिखाएँ
Console.WriteLine("User Password: " + encryptionDetails.UserPassword);
Console.WriteLine("Owner Password: " + encryptionDetails.OwnerPassword);
// एन्क्रिप्शन मोड दिखाएँ: RC4_40 या RC4_128
Console.WriteLine("Encryption Algorithm: " + encryptionDetails.EncryptionAlgorithm);
Console.WriteLine("Permissions: " + encryptionDetails.Permissions);

var options = new PdfSaveOptions
{
    EncryptionDetails = encryptionDetails
};

// निर्दिष्ट एन्क्रिप्शन विवरण के साथ प्रोजेक्ट सहेजें
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### संबंधित देखें

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


