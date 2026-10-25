---
title: "XpsOptions.RenderMetafileAsBitmap"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "XpsOptions प्रॉपर्टी। यह मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि एक मेटाफाइल को बिटमैप के रूप में रेंडर किया जाना चाहिए या नहीं।"
type: docs
weight: 20
url: /hi/net/aspose.tasks.saving/xpsoptions/rendermetafileasbitmap/
---
## XpsOptions.RenderMetafileAsBitmap property

एक मेटाफाइल को बिटमैप के रूप में रेंडर किया जाना चाहिए या नहीं, यह संकेत देने वाला मान प्राप्त करता है या सेट करता है।

```csharp
public bool RenderMetafileAsBitmap { get; set; }
```

## उदाहरण

दिखाता है कि प्रोजेक्ट को XPS फ़ाइल के रूप में कैसे सहेजा जाए।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// XPS सेव विकल्प बनाएं और पैरामीटर समायोजित करें
var options = new XpsOptions
{
    RenderMetafileAsBitmap = true
};

project.Save(OutDir + "UseSvgOptions_out.xps", options);
```

### संबंधित देखें

* class [XpsOptions](../)
* namespace [Aspose.Tasks.Saving](../../xpsoptions/)
* assembly [Aspose.Tasks](../../../)


