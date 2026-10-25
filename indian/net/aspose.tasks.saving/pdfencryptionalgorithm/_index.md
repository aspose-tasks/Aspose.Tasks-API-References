---
title: "एनम PdfEncryptionAlgorithm"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Saving.PdfEncryptionAlgorithm एनम। PDF दस्तावेज़ को एन्क्रिप्ट करने के लिए उपयोग किए जाने वाले एन्क्रिप्शन एल्गोरिदम को निर्दिष्ट करता है"
type: docs
weight: 2100
url: /hi/net/aspose.tasks.saving/pdfencryptionalgorithm/
---
## PdfEncryptionAlgorithm enumeration

PDF दस्तावेज़ को एन्क्रिप्ट करने के लिए उपयोग किए जाने वाले एन्क्रिप्शन एल्गोरिद्म को निर्दिष्ट करता है।

```csharp
public enum PdfEncryptionAlgorithm
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| RC4_40 | `0` | PDF दस्तावेज़ को एन्क्रिप्ट करने के लिए उपयोग किए जाने वाले एन्क्रिप्शन एल्गोरिद्म को निर्दिष्ट करता है। |
| RC4_128 | `1` | PDF दस्तावेज़ को एन्क्रिप्ट करने के लिए उपयोग किए जाने वाले एन्क्रिप्शन एल्गोरिद्म को निर्दिष्ट करता है। |

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


