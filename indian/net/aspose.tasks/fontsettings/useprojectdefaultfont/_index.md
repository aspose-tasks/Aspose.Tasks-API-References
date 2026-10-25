---
title: "FontSettings.UseProjectDefaultFont"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "FontSettings प्रॉपर्टी। एक मान प्राप्त करता या सेट करता है जो दर्शाता है कि रेंडरिंग के लिए डिफ़ॉल्ट फ़ॉन्ट उपयोग किया जाना चाहिए या नहीं।"
type: docs
weight: 40
url: /hi/net/aspose.tasks/fontsettings/useprojectdefaultfont/
---
## FontSettings.UseProjectDefaultFont property

रेंडरिंग के लिए डिफ़ॉल्ट फ़ॉन्ट का उपयोग किया जाना चाहिए या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है।

```csharp
public bool UseProjectDefaultFont { get; set; }
```

## टिप्पणियाँ

जब मान False है और DefaultFontName निर्दिष्ट किया गया है, तो रेंडरिंग इंजन DefaultFontName द्वारा निर्दिष्ट फ़ॉन्ट को फॉलबैक फ़ॉन्ट के रूप में उपयोग करेगा। अन्यथा 'Arial' (यदि स्थापित है) या 'Generic Sans Serif' फ़ॉन्ट को फॉलबैक फ़ॉन्ट के रूप में उपयोग किया जाता है। फॉलबैक फ़ॉन्ट प्रोजेक्ट व्यू के रेंडरिंग के दौरान उपयोग किया जाता है जब किसी टेक्स्ट स्टाइल में ऐसा फ़ॉन्ट संदर्भित होता है जो वर्तमान ऑपरेटिंग सिस्टम पर स्थापित नहीं है। फ़ॉन्ट रिज़ॉल्यूशन पर अधिक नियंत्रण के लिए आप [`FontResolveCallback`](../fontresolvecallback/) कॉलबैक का उपयोग कर सकते हैं।

## उदाहरण

कस्टम फ़ॉन्ट सेट करने का तरीका दिखाता है जो आउटपुट PDF के प्रिंट में उपयोग होगा।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart, FitContent = true
                  };

options.FontSettings.UseProjectDefaultFont = false;
options.FontSettings.DefaultFontName = "Segoe UI Black";
project.Save(OutDir + "CreateProject2_out.pdf", options);
```

### संबंधित देखें

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


