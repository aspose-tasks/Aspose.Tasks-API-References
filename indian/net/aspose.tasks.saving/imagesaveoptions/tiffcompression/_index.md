---
title: "ImageSaveOptions.TiffCompression"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ImageSaveOptions प्रॉपर्टी। उत्पन्न छवियों को TIFF फ़ॉर्मेट में सहेजते समय लागू करने के लिए संपीड़न प्रकार को प्राप्त करता है या सेट करता है"
type: docs
weight: 90
url: /hi/net/aspose.tasks.saving/imagesaveoptions/tiffcompression/
---
## ImageSaveOptions.TiffCompression property

जनरेटेड इमेज़ को TIFF फ़ॉर्मेट में सहेजते समय लागू किए जाने वाले कम्प्रेशन प्रकार को प्राप्त करता है या सेट करता है।

```csharp
public TiffCompression TiffCompression { get; set; }
```

## टिप्पणियाँ

केवल TIFF में सहेजते समय प्रभावी होता है। डिफ़ॉल्ट मान `LZW` है।

## उदाहरण

दिखाता है कि आउटपुट TIFF फ़ाइलों की TIFF संपीड़न कैसे सेट करें।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// TIFF संपीड़न को नियंत्रित करने के लिए हम ImageSaveOptions.TiffCompression प्रॉपर्टी का उपयोग कर सकते हैं।
var options = new ImageSaveOptions(SaveFileFormat.Tiff)
{
    TiffCompression = TiffCompression.Lzw
};

project.Save(OutDir + "SaveProjectAsTiff_out.tif", options);
```

### संबंधित देखें

* enum [TiffCompression](../../tiffcompression/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


