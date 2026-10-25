---
title: "ImageSaveOptions.ReduceFooterGap"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ImageSaveOptions प्रॉपर्टी। यह दर्शाने वाला मान प्राप्त करता है या सेट करता है कि अंतिम कार्य और फुटर के बीच का गैप घटाया जाना चाहिए या नहीं"
type: docs
weight: 80
url: /hi/net/aspose.tasks.saving/imagesaveoptions/reducefootergap/
---
## ImageSaveOptions.ReduceFooterGap property

एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि अंतिम कार्य और फुटर के बीच का अंतराल घटाया जाना चाहिए या नहीं।

```csharp
public bool ReduceFooterGap { get; set; }
```

## उदाहरण

दिखाता है कि अंतिम कार्य और फुटर के बीच के गैप को घटाने के लिए मान कैसे सेट करें।

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// कार्य की सूची और फुटर के बीच के गैप को घटाने के लिए ReduceFooterGap प्रॉपर्टी का उपयोग करें
var imageSaveOptions = new ImageSaveOptions(SaveFileFormat.Png)
                           {
                               ReduceFooterGap = true, /* set to true */ 
                               RenderToSinglePage = false,
                               PageSize = PageSize.A0,
                               Timescale = Timescale.Days
                           };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.png", imageSaveOptions);
```

### संबंधित देखें

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


