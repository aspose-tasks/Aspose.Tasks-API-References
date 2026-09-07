---
title: "क्लास PageViewSettings"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.PageViewSettings क्लास। प्रोजेक्ट व्यू के लिए प्रिंटिंग सेटिंग्स का प्रतिनिधित्व करता है"
type: docs
weight: 3260
url: /hi/net/aspose.tasks.visualization/pageviewsettings/
---
## PageViewSettings class

प्रोजेक्ट दृश्य के लिए प्रिंटिंग सेटिंग्स को दर्शाता है।

```csharp
public class PageViewSettings
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [PageViewSettings](pageviewsettings/)() | डिफ़ॉल्ट कन्स्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [FirstColumnsCount](../../aspose.tasks.visualization/pageviewsettings/firstcolumnscount/) { get; set; } | सभी पृष्ठों पर प्रिंट होने वाले पहले कॉलमों की संख्या प्राप्त करता है या सेट करता है। |
| [FitTimescaleToEndOfPage](../../aspose.tasks.visualization/pageviewsettings/fittimescaletoendofpage/) { get; set; } | प्रिंट करते समय टाइमस्केल को पृष्ठ के अंत तक फिट करने का संकेत देने वाला मान प्राप्त करता है या सेट करता है। |
| [PrintAllSheetColumns](../../aspose.tasks.visualization/pageviewsettings/printallsheetcolumns/) { get; set; } | किसी व्यू की सभी शीट कॉलमों को प्रिंट करने का संकेत देने वाला मान प्राप्त करता है या सेट करता है। |
| [PrintBlankPages](../../aspose.tasks.visualization/pageviewsettings/printblankpages/) { get; set; } | किसी व्यू के खाली पृष्ठों को प्रिंट करने का संकेत देने वाला मान प्राप्त करता है या सेट करता है। |
| [PrintFirstColumnsCountOnAllPages](../../aspose.tasks.visualization/pageviewsettings/printfirstcolumnscountonallpages/) { get; set; } | सभी पृष्ठों पर निर्दिष्ट संख्या में पहले कॉलमों को प्रिंट करने का संकेत देने वाला मान प्राप्त करता है या सेट करता है। |
| [PrintNotes](../../aspose.tasks.visualization/pageviewsettings/printnotes/) { get; set; } | नोट्स को प्रिंट करने का संकेत देने वाला मान प्राप्त करता है या सेट करता है। |

## उदाहरण

दिखाता है कि टास्क, रिसोर्स, असाइनमेंट नोट्स को अलग पृष्ठ पर कैसे प्रिंट किया जाए।

```csharp
var project = new Project(DataDir + "Input.mpp");

// सभी पृष्ठों पर प्रिंट होने वाले पहले कॉलमों की संख्या सेट करें
project.DefaultView.PageInfo.PageViewSettings.FirstColumnsCount = 2;

// नोट्स को प्रिंट करने का संकेत देने वाला मान सेट करें।
project.DefaultView.PageInfo.PageViewSettings.PrintNotes = true;

// प्रिंट करते समय टाइमस्केल को पृष्ठ के अंत तक फिट करने का संकेत देने वाला मान सेट करें।
project.DefaultView.PageInfo.PageViewSettings.FitTimescaleToEndOfPage = true;

// किसी व्यू की सभी शीट कॉलमों को प्रिंट करने का संकेत देने वाला मान सेट करें
project.DefaultView.PageInfo.PageViewSettings.PrintAllSheetColumns = true;

// किसी व्यू के खाली पृष्ठों को प्रिंट करने का संकेत देने वाला मान सेट करें
project.DefaultView.PageInfo.PageViewSettings.PrintBlankPages = false;

// सभी पृष्ठों पर निर्दिष्ट संख्या में पहले कॉलम प्रिंट करने का संकेत देने वाला मान सेट करें
project.DefaultView.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

project.Save(OutDir + "ProjectWithComments_out.pdf", SaveFileFormat.Pdf);
```

### संबंधित देखें

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


