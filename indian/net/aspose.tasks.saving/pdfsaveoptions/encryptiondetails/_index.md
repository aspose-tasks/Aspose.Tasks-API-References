---
title: "PdfSaveOptions.EncryptionDetails"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PdfSaveOptions प्रॉपर्टी। एन्क्रिप्शन विवरण को प्राप्त या सेट करता है। यदि सेट नहीं किया गया तो कोई एन्क्रिप्शन नहीं किया जाएगा।"
type: docs
weight: 40
url: /hi/net/aspose.tasks.saving/pdfsaveoptions/encryptiondetails/
---
## PdfSaveOptions.EncryptionDetails property

एन्क्रिप्शन विवरण प्राप्त करता है या सेट करता है। यदि सेट नहीं किया गया, तो कोई एन्क्रिप्शन नहीं किया जाएगा।

```csharp
public PdfEncryptionDetails EncryptionDetails { get; set; }
```

## उदाहरण

PDF दस्तावेज़ के एन्क्रिप्शन विवरण को सेट करने का तरीका दर्शाता है। यदि सेट नहीं किया गया, तो कोई एन्क्रिप्शन नहीं किया जाएगा।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var encryptionDetails = new PdfEncryptionDetails("userPassword", "ownerPassword", PdfEncryptionAlgorithm.RC4_128);

var options = new PdfSaveOptions();

// PDF दस्तावेज़ के एन्क्रिप्शन विवरण को सेट करें।
options.EncryptionDetails = encryptionDetails;

// अतिरिक्त गुणों को समायोजित करें
// उस <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> को सेट करें जिसमें दस्तावेज़ सहेजा जाएगा।
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithEncryptionDetails_out.pdf", options);
```

### संबंधित देखें

* class [PdfEncryptionDetails](../../pdfencryptiondetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


