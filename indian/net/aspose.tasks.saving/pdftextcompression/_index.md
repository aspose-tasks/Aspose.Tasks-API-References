---
title: "एन्यूम PdfTextCompression"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Saving.PdfTextCompression एन्यूम। PDF फ़ाइल में सभी सामग्री पर, छवियों को छोड़कर, लागू की जाने वाली संपीड़न प्रकार को निर्दिष्ट करता है।"
type: docs
weight: 2140
url: /hi/net/aspose.tasks.saving/pdftextcompression/
---
## PdfTextCompression enumeration

छवियों को छोड़कर PDF फ़ाइल की सभी सामग्री पर लागू होने वाले संपीड़न प्रकार को निर्दिष्ट करता है।

```csharp
public enum PdfTextCompression
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| None | `0` | कोई संपीड़न नहीं। |
| Flate | `1` | Flate संपीड़न। |

## उदाहरण

दिखाता है कि सभी कंटेंट स्ट्रीम्स के लिए, छवियों को छोड़कर, किस प्रकार का संपीड़न सेट किया जाए।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// सभी कंटेंट स्ट्रीम्स के लिए, छवियों को छोड़कर, उपयोग किए जाने वाले संपीड़न प्रकार को सेट करें
options.TextCompression = PdfTextCompression.Flate;

// अतिरिक्त गुणों को समायोजित करें
// उस <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> को सेट करें जिसमें दस्तावेज़ सहेजा जाएगा।
options.PresentationFormat = PresentationFormat.GanttChart;

// उत्पन्न PDF दस्तावेज़ के लिए इच्छित अनुपालन स्तर सेट करें
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithTextCompression_out.pdf", options);
```

### संबंधित देखें

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


