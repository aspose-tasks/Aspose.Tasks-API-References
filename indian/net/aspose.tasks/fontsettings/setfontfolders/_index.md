---
title: "FontSettings.SetFontFolders"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "FontSettings मेथड। प्रोजेक्ट व्यू रेंडर करते समय Aspose.Tasks द्वारा TrueType फ़ॉन्ट्स खोजने के लिए फ़ोल्डर्स सेट करता है।"
type: docs
weight: 50
url: /hi/net/aspose.tasks/fontsettings/setfontfolders/
---
## FontSettings.SetFontFolders method

प्रोजेक्ट व्यू को रेंडर करते समय Aspose.Tasks द्वारा TrueType फ़ॉन्ट खोजने वाले फ़ोल्डरों को सेट करता है।

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fontFolders | String[] | TrueType फ़ॉन्ट्स वाले फ़ोल्डर्स की एक एरे। |
| recursive | Boolean | यदि true हो, तो निर्दिष्ट फ़ोल्डर्स को पुनरावर्ती रूप से स्कैन किया जाएगा। |

## उदाहरण

कस्टम फ़ॉन्ट फ़ोल्डर सेट करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

// खुले प्रोजेक्ट में उपयोग किए गए सभी फ़ॉन्ट्स की TrueType फ़ाइलें MyFonts फ़ोल्डर में स्थित होनी चाहिए।
options.FontSettings.SetFontFolders(new string[] { "c:\\MyFonts"}, true);

project.Save(OutDir + "EstimatedMilestoneTasks_out4.pdf", options);
```

### संबंधित देखें

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


