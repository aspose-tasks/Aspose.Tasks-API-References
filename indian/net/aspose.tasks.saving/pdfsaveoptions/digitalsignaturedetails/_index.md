---
title: "PdfSaveOptions.DigitalSignatureDetails"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PdfSaveOptions प्रॉपर्टी। डिजिटल सिग्नेचर विवरण को प्राप्त या सेट करता है। यदि सेट नहीं किया गया तो कोई साइनिंग नहीं होगी।"
type: docs
weight: 30
url: /hi/net/aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/
---
## PdfSaveOptions.DigitalSignatureDetails property

डिजिटल सिग्नेचर विवरण प्राप्त करता है या सेट करता है। यदि सेट नहीं किया गया, तो कोई साइनिंग नहीं होगी।

```csharp
public PdfDigitalSignatureDetails DigitalSignatureDetails { get; set; }
```

## उदाहरण

डिजिटल सिग्नेचर विवरण को सेट करने का तरीका दर्शाता है। यदि सेट नहीं किया गया, तो कोई साइनिंग नहीं होगी।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
var certificate = new X509Certificate2();

// डिजिटल सिग्नेचर विवरण सेट करें। यदि सेट नहीं किया गया, तो कोई साइनिंग नहीं होगी।
options.DigitalSignatureDetails = new PdfDigitalSignatureDetails(
    certificate,
    "reason",
    "location",
    new DateTime(2019, 1, 1),
    PdfDigitalSignatureHashAlgorithm.Sha1);

// अतिरिक्त गुणों को समायोजित करें
// उस <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> को सेट करें जिसमें दस्तावेज़ सहेजा जाएगा।
options.PresentationFormat = PresentationFormat.GanttChart;

// उत्पन्न PDF दस्तावेज़ के लिए इच्छित अनुपालन स्तर सेट करें
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithDigitalSignatureDetails_out.pdf", options);
```

### संबंधित देखें

* class [PdfDigitalSignatureDetails](../../pdfdigitalsignaturedetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


