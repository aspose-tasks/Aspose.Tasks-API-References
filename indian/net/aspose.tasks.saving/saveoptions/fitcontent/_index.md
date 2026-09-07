---
title: "SaveOptions.FitContent"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveOptions प्रॉपर्टी। प्राप्त करता है या सेट करता है एक मान जो दर्शाता है कि क्या पंक्ति की ऊँचाई को उसके कंटेंट में फिट होने के लिए बढ़ाया जाना चाहिए।"
type: docs
weight: 50
url: /hi/net/aspose.tasks.saving/saveoptions/fitcontent/
---
## SaveOptions.FitContent property

एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि पंक्ति की ऊँचाई को उसकी सामग्री के अनुसार बढ़ाया जाना चाहिए या नहीं।

```csharp
public bool FitContent { get; set; }
```

## उदाहरण

दिखाता है कि कैसे विकल्प सेट किया जाए कि पंक्ति की ऊँचाई उसकी सामग्री को फिट करने के लिए बढ़ाई जानी चाहिए या नहीं।

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // फ़िट कंटेंट विकल्प को true सेट करें
    FitContent = true,
    Timescale = Timescale.Months,
    PresentationFormat = PresentationFormat.TaskUsage
};
project.Save(OutDir + "FitContentsToCellSize_out.pdf", options);
```

### संबंधित देखें

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


