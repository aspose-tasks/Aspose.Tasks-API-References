---
title: "ImageSaveOptions.ImageSaveOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ImageSaveOptions कंस्ट्रक्टर। ImageSaveOptions क्लास का नया इंस्टेंस इनिशियलाइज़ करता है जिसका उपयोग रेंडर की गई छवियों को TIFF, PNG, BMP या JPEG फ़ॉर्मेट में सहेजने के लिए किया जा सकता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks.saving/imagesaveoptions/imagesaveoptions/
---
## ImageSaveOptions constructor

एक नया इंस्टेंस इनिशियलाइज़ करता है [`ImageSaveOptions`](../) क्लास का, जिसका उपयोग रेंडर की गई छवियों को TIFF, PNG, BMP या JPEG फ़ॉर्मेट में सहेजने के लिए किया जा सकता है।

```csharp
public ImageSaveOptions(SaveFileFormat saveFormat)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| saveFormat | SaveFileFormat | TIFF, PNG, BMP या JPEG[`SaveFileFormat`](../../savefileformat/) हो सकता है। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentException | *saveFormat* के अवैध होने पर थ्रो किया जाता है। वैध मान TIFF, PNG, BMP या JPEG हैं। |

## उदाहरण

दिखाता है कि प्रोजेक्ट को इमेज़ के रूप में स्ट्रीम में कैसे सहेजा जाए।

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // ImageSaveOptions का उपयोग करके हम प्रोजेक्ट को इमेज़ फ़ॉर्मेट में सहेजते हैं
    project.Save(stream, options);
}
```

### संबंधित देखें

* enum [SaveFileFormat](../../savefileformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


