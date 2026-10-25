---
title: "PdfSaveOptions.Compliance"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PdfSaveOptions प्रॉपर्टी। उत्पन्न PDF दस्तावेज़ के लिए वांछित अनुपालन स्तर को प्राप्त या सेट करता है। डिफ़ॉल्ट Pdf15 है।"
type: docs
weight: 20
url: /hi/net/aspose.tasks.saving/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

जनरेटेड PDF दस्तावेज़ के लिए वांछित अनुपालन स्तर प्राप्त करता है या सेट करता है। डिफ़ॉल्ट Pdf15 है।

```csharp
public PdfCompliance Compliance { get; set; }
```

## उदाहरण

जेनरेटेड PDF दस्तावेज़ के लिए इच्छित अनुपालन स्तर कैसे सेट करें, यह दिखाता है।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// उत्पन्न PDF दस्तावेज़ के लिए इच्छित अनुपालन स्तर सेट करें
// डिफ़ॉल्ट <see cref=\"PdfCompliance.Pdf15\"/> प्रकार है
options.Compliance = PdfCompliance.PdfA1b;

// अतिरिक्त गुणों को समायोजित करें
// उस <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> को सेट करें जिसमें दस्तावेज़ सहेजा जाएगा।
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithPdfCompliance_out.pdf", options);
```

### संबंधित देखें

* enum [PdfCompliance](../../pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


