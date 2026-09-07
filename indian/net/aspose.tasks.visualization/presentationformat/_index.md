---
title: "Enum PresentationFormat"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.PresentationFormat enum. प्रस्तुति प्रारूप के लिए एन्यूमरेशन"
type: docs
weight: 3270
url: /hi/net/aspose.tasks.visualization/presentationformat/
---
## PresentationFormat enumeration

प्रेजेंटेशन फ़ॉर्मेट के लिए एन्यूमरेशन।

```csharp
public enum PresentationFormat
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| GanttChart | `0` | गैंट चार्ट प्रस्तुति प्रारूप। |
| TaskUsage | `1` | टास्क उपयोग प्रस्तुति प्रारूप। |
| ResourceUsage | `2` | संसाधन उपयोग प्रस्तुति प्रारूप। |
| ResourceSheet | `3` | संसाधन शीट प्रस्तुति प्रारूप। |
| TaskSheet | `4` | टास्क शीट प्रस्तुति प्रारूप। |

## उदाहरण

संसाधन शीट दृश्य को रेंडर करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "ResourceSheetView.mpp");

SaveOptions options = new PdfSaveOptions();

// प्रस्तुति प्रारूप को संसाधन शीट पर सेट करें
options.PresentationFormat = PresentationFormat.ResourceSheet;
project.Save(OutDir + "ResourceSheetView_out.pdf", options);
```

### संबंधित देखें

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


