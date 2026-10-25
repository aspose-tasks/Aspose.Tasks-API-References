---
title: "PdfDigitalSignatureDetails.PdfDigitalSignatureDetails"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PdfDigitalSignatureDetails कंस्ट्रक्टर। PdfDigitalSignatureDetails क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks.saving/pdfdigitalsignaturedetails/pdfdigitalsignaturedetails/
---
## PdfDigitalSignatureDetails constructor

एक नया [`PdfDigitalSignatureDetails`](../) क्लास का इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public PdfDigitalSignatureDetails(X509Certificate2 certificate, string reason, string location, 
    DateTime signatureDate, PdfDigitalSignatureHashAlgorithm hashAlgorithm)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रमाणपत्र | X509Certificate2 | साइन करने के लिए X509Certificate2 इंस्टेंस। |
| कारण | स्ट्रिंग | हस्ताक्षर करने का कारण। |
| स्थान | स्ट्रिंग | हस्ताक्षर करने का स्थान। |
| signatureDate | DateTime | हस्ताक्षर की तिथि। |
| hashAlgorithm | PdfDigitalSignatureHashAlgorithm | हस्ताक्षर का हैश एल्गोरिदम। |

## उदाहरण

दिखाता है कि PDF डिजिटल सिग्नेचर विवरणों के साथ कैसे काम किया जाए।

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new PdfSaveOptions();

var certificate = new X509Certificate2();

// PDF सिग्नेचर विवरण बनाएं
var signatureDetails = new PdfDigitalSignatureDetails(
    // प्रमाणपत्र निर्दिष्ट करें
    certificate, 
    // हस्ताक्षर करने का कारण निर्दिष्ट करें
    "reason",
    // हस्ताक्षर करने का स्थान निर्दिष्ट करें
    "location", 
    // हस्ताक्षर करने की तिथि निर्दिष्ट करें
    new DateTime(2019, 1, 1), 
    // हस्ताक्षर के हैश एल्गोरिद्म को निर्दिष्ट करें
    PdfDigitalSignatureHashAlgorithm.Sha1);

Console.WriteLine("Certificate: " + signatureDetails.Certificate);
Console.WriteLine("Reason: " + signatureDetails.Reason);
Console.WriteLine("Location: " + signatureDetails.Location);
Console.WriteLine("Signature Date: " + signatureDetails.SignatureDate);
Console.WriteLine("Hash Algorithm: " + signatureDetails.HashAlgorithm);

// डिजिटल सिग्नेचर विवरण सेट करें
options.DigitalSignatureDetails = signatureDetails;

// निर्दिष्ट एन्क्रिप्शन विवरण के साथ प्रोजेक्ट सहेजें
project.Save(OutDir + "WorkWithPdfEncryptionDetails_out.pdf", options);
```

### संबंधित देखें

* enum [PdfDigitalSignatureHashAlgorithm](../../pdfdigitalsignaturehashalgorithm/)
* class [PdfDigitalSignatureDetails](../)
* namespace [Aspose.Tasks.Saving](../../pdfdigitalsignaturedetails/)
* assembly [Aspose.Tasks](../../../)


