---
title: "PageViewSettings.PrintAllSheetColumns"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PageViewSettings प्रॉपर्टी। व्यू की सभी शीट कॉलम को प्रिंट करने का संकेत देने वाले मान को प्राप्त करता है या सेट करता है"
type: docs
weight: 40
url: /hi/net/aspose.tasks.visualization/pageviewsettings/printallsheetcolumns/
---
## PageViewSettings.PrintAllSheetColumns property

किसी व्यू की सभी शीट कॉलमों को प्रिंट करने का संकेत देने वाला मान प्राप्त करता है या सेट करता है।

```csharp
public bool PrintAllSheetColumns { get; set; }
```

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

* class [PageViewSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pageviewsettings/)
* assembly [Aspose.Tasks](../../../)


