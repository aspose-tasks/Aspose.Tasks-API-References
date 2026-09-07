---
title: "एनम TiffCompression"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Saving.TiffCompression enum. पेज को TIFF फ़ॉर्मेट में सहेजते समय लागू करने के लिए संपीड़न का प्रकार निर्दिष्ट करता है।"
type: docs
weight: 2250
url: /hi/net/aspose.tasks.saving/tiffcompression/
---
## TiffCompression enumeration

TIFF फ़ॉर्मेट में पेज सहेजते समय लागू करने वाले संपीड़न प्रकार को निर्दिष्ट करता है।

```csharp
public enum TiffCompression
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| None | `1` | कोई संपीड़न नहीं निर्दिष्ट करता है। |
| Rle | `2` | RLE संपीड़न योजना को निर्दिष्ट करता है। |
| Ccitt3 | `3` | CCITT3 संपीड़न योजना को निर्दिष्ट करता है। |
| Ccitt4 | `4` | CCITT4 संपीड़न योजना को निर्दिष्ट करता है। |
| Lzw | `5` | LZW संपीड़न योजना को निर्दिष्ट करता है। |

## उदाहरण

RLE संपीड़न मोड का उपयोग करके TIFF फ़ॉर्मेट में रेंडर करना कैसे दिखाता है।

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Tiff);

// Rle संपीड़न के साथ प्रोजेक्ट सहेजें
options.TiffCompression = TiffCompression.Rle;
project.Save(OutDir + "RenderMultipageTIFF_comp_rle_out.tif", options);
```

### संबंधित देखें

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


