---
title: "ImageSaveOptions.VerticalResolution"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ImageSaveOptions प्रॉपर्टी। dpi में वर्टिकल रेज़ोल्यूशन को प्राप्त या सेट करता है।"
type: docs
weight: 100
url: /hi/net/aspose.tasks.saving/imagesaveoptions/verticalresolution/
---
## ImageSaveOptions.VerticalResolution property

डॉट्स प्रति इंच (dpi) में लंबवत रिज़ॉल्यूशन प्राप्त करता है या सेट करता है।

```csharp
public float VerticalResolution { get; set; }
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


