---
title: "XpsOptions.XpsOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "XpsOptions constructor. नई XpsOptions क्लास की एक नई इंस्टेंस को इनिशियलाइज़ करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks.saving/xpsoptions/xpsoptions/
---
## XpsOptions constructor

नई [`XpsOptions`](../) क्लास की एक नई इंस्टेंस को इनिशियलाइज़ करता है।

```csharp
public XpsOptions()
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


