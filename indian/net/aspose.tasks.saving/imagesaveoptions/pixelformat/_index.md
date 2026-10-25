---
title: "ImageSaveOptions.PixelFormat"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ImageSaveOptions प्रॉपर्टी। छवि में प्रत्येक पिक्सेल के लिए रंग डेटा के फ़ॉर्मेट को प्राप्त करता है या सेट करता है"
type: docs
weight: 70
url: /hi/net/aspose.tasks.saving/imagesaveoptions/pixelformat/
---
## ImageSaveOptions.PixelFormat property

इमेज़ में प्रत्येक पिक्सेल के लिए कलर डेटा का फ़ॉर्मेट प्राप्त करता है या सेट करता है।

```csharp
public PixelFormat PixelFormat { get; set; }
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


