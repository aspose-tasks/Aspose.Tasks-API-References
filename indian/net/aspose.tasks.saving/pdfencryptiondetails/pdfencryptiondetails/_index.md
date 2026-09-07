---
title: "PdfEncryptionDetails.PdfEncryptionDetails"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PdfEncryptionDetails कंस्ट्रक्टर। PdfEncryptionDetails क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks.saving/pdfencryptiondetails/pdfencryptiondetails/
---
## PdfEncryptionDetails constructor

[`PdfEncryptionDetails`](../) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public PdfEncryptionDetails(string userPassword, string ownerPassword, 
    PdfEncryptionAlgorithm encryptionAlgorithm)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| userPassword | स्ट्रिंग | उपयोगकर्ता पासवर्ड जो संरक्षित दस्तावेज़ खोलने की अनुमति देता है। |
| ownerPassword | स्ट्रिंग | ओनर पासवर्ड जो संरक्षित दस्तावेज़ खोलने की अनुमति देता है। |
| encryptionAlgorithm | PdfEncryptionAlgorithm | [`PdfEncryptionAlgorithm`](../../pdfencryptionalgorithm/) इंस्टेंस जो एन्क्रिप्शन एल्गोरिदम दर्शाता है। |

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

* enum [PdfEncryptionAlgorithm](../../pdfencryptionalgorithm/)
* class [PdfEncryptionDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfencryptiondetails/)
* assembly [Aspose.Tasks](../../../)


