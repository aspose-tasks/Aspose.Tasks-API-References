---
title: "PdfDigitalSignatureDetails.HashAlgorithm"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PdfDigitalSignatureDetails प्रॉपर्टी। हैश एल्गोरिदम प्राप्त करता है या सेट करता है"
type: docs
weight: 30
url: /hi/net/aspose.tasks.saving/pdfdigitalsignaturedetails/hashalgorithm/
---
## PdfDigitalSignatureDetails.HashAlgorithm property

हैश एल्गोरिदम को प्राप्त करता है या सेट करता है।

```csharp
public PdfDigitalSignatureHashAlgorithm HashAlgorithm { get; set; }
```

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


