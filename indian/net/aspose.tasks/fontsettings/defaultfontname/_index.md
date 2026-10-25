---
title: "FontSettings.DefaultFontName"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "FontSettings प्रॉपर्टी। रेंडरिंग के लिए डिफ़ॉल्ट या फॉलबैक फ़ॉन्ट प्राप्त करता या सेट करता है।"
type: docs
weight: 20
url: /hi/net/aspose.tasks/fontsettings/defaultfontname/
---
## FontSettings.DefaultFontName property

रेंडरिंग के लिए डिफ़ॉल्ट (या फॉलबैक) फ़ॉन्ट प्राप्त करता है या सेट करता है।

```csharp
public string DefaultFontName { get; set; }
```

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


