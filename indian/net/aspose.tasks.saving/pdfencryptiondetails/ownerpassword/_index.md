---
title: "PdfEncryptionDetails.OwnerPassword"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PdfEncryptionDetails प्रॉपर्टी। Owner पासवर्ड प्राप्त करता है या सेट करता है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks.saving/pdfencryptiondetails/ownerpassword/
---
## PdfEncryptionDetails.OwnerPassword property

ओनर पासवर्ड को प्राप्त करता है या सेट करता है।

```csharp
public string OwnerPassword { get; set; }
```

## टिप्पणियाँ

सही ओनर पासवर्ड के साथ दस्तावेज़ खोलने से (मान लेते हैं कि यह उपयोगकर्ता पासवर्ड के समान नहीं है) दस्तावेज़ तक पूर्ण (ओनर) पहुंच मिलती है। यह असीमित पहुंच दस्तावेज़ के पासवर्ड और एक्सेस अनुमतियों को बदलने की क्षमता भी शामिल करती है।

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

* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


