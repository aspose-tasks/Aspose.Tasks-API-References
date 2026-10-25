---
title: "PdfSaveOptions.TextCompression"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PdfSaveOptions प्रॉपर्टी। वह संपीड़न प्रकार प्राप्त करता है या सेट करता है जिसे सभी कंटेंट स्ट्रीम्स (छवियों को छोड़कर) के लिए उपयोग किया जाएगा। डिफ़ॉल्ट Flate है।"
type: docs
weight: 100
url: /hi/net/aspose.tasks.saving/pdfsaveoptions/textcompression/
---
## PdfSaveOptions.TextCompression property

इमेज़ को छोड़कर सभी कंटेंट स्ट्रीम्स के लिए उपयोग किए जाने वाले कम्प्रेशन प्रकार को प्राप्त करता है या सेट करता है। डिफ़ॉल्ट Flate है।

```csharp
public PdfTextCompression TextCompression { get; set; }
```

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

* enum [PdfTextCompression](../../pdftextcompression/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


