---
title: "ImageSaveOptions.JpegQuality"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ImageSaveOptions प्रॉपर्टी। JPEG गुणवत्ता को प्राप्त करता है या सेट करता है। अनुमत मान सीमा 0..100 है"
type: docs
weight: 40
url: /hi/net/aspose.tasks.saving/imagesaveoptions/jpegquality/
---
## ImageSaveOptions.JpegQuality property

JPEG क्वालिटी प्राप्त करता है या सेट करता है। अनुमत मान सीमा 0..100 है।

```csharp
public int JpegQuality { get; set; }
```

## उदाहरण

दिखाता है कि आउटपुट JPEG फ़ाइलों की JPEG गुणवत्ता कैसे सेट करें।

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// JPEG गुणवत्ता को बदलने के लिए आप ImageSaveOptions.JpegQuality प्रॉपर्टी का उपयोग कर सकते हैं।
// अनुमत मान सीमा 0..100 है।
var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
{
    JpegQuality = 50
};

project.Save(OutDir + "SaveProjectAsJPEG_out.jpeg", options);
```

### संबंधित देखें

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


