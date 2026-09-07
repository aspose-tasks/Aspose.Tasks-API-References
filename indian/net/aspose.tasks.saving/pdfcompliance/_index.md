---
title: "एनम PdfCompliance"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Saving.PdfCompliance एनम। आउटपुट फ़ाइल के लिए PDF अनुपालन स्तर निर्दिष्ट करता है।"
type: docs
weight: 2070
url: /hi/net/aspose.tasks.saving/pdfcompliance/
---
## PdfCompliance enumeration

आउटपुट फ़ाइल के लिए PDF अनुपालन स्तर निर्दिष्ट करता है।

```csharp
public enum PdfCompliance
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Pdf15 | `0` | PDF/15 अनुपालन स्तर। |
| PdfA1a | `1` | PDF/A-1a अनुपालन स्तर। |
| PdfA1b | `2` | PDF/A-1b अनुपालन स्तर। |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


