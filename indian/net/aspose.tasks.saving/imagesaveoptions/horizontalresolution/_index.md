---
title: "ImageSaveOptions.HorizontalResolution"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ImageSaveOptions प्रॉपर्टी। क्षैतिज रिज़ॉल्यूशन को dpi में प्राप्त करता है या सेट करता है"
type: docs
weight: 30
url: /hi/net/aspose.tasks.saving/imagesaveoptions/horizontalresolution/
---
## ImageSaveOptions.HorizontalResolution property

डॉट्स प्रति इंच (dpi) में क्षैतिज रिज़ॉल्यूशन प्राप्त करता है या सेट करता है।

```csharp
public float HorizontalResolution { get; set; }
```

## उदाहरण

इमेज फ़ॉर्मेट में रूपांतरण के दौरान उपयोग किए जाने वाले पिक्सेल फ़ॉर्मेट को सेट करने का तरीका दर्शाता है।

```csharp
var project = new Project(DataDir + "Project1.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Tiff);
options.HorizontalResolution = 72;
options.VerticalResolution = 72;
options.PixelFormat = PixelFormat.Format24bppRgb;
project.Save(OutDir + "RenderProjectDataToFormat24bppRgb_out.tif", options);
```

### संबंधित देखें

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


