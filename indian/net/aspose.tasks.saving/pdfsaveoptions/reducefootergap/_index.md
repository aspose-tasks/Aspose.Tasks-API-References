---
title: "PdfSaveOptions.ReduceFooterGap"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PdfSaveOptions प्रॉपर्टी। यह निर्धारित करने के लिए मान प्राप्त या सेट करता है कि अंतिम कार्य और फुटर के बीच का अंतराल घटाया जाना चाहिए या नहीं।"
type: docs
weight: 80
url: /hi/net/aspose.tasks.saving/pdfsaveoptions/reducefootergap/
---
## PdfSaveOptions.ReduceFooterGap property

एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि अंतिम कार्य और फुटर के बीच का अंतराल घटाया जाना चाहिए या नहीं।

```csharp
public bool ReduceFooterGap { get; set; }
```

## उदाहरण

PDF आउटपुट फ़ाइलों में अंतिम कार्य और फुटर के बीच के अंतराल को घटाने की आवश्यकता को दर्शाने वाले मान को सेट करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions { ReduceFooterGap = true, PageSize = PageSize.A0, Timescale = Timescale.Days };

project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.pdf", options);
```

### संबंधित देखें

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


