---
title: "PageSettings.PaperSize"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PageSettings प्रॉपर्टी। कागज़ का आकार प्राप्त करता है या सेट करता है। यह PrinterPaperSize एनेमरेशन के मानों में से एक हो सकता है।"
type: docs
weight: 70
url: /hi/net/aspose.tasks.visualization/pagesettings/papersize/
---
## PageSettings.PaperSize property

कागज़ का आकार प्राप्त करता है या सेट करता है। यह [`PrinterPaperSize`](../../printerpapersize/) एनेमरेशन के मानों में से एक हो सकता है।

```csharp
public PrinterPaperSize PaperSize { get; set; }
```

## उदाहरण

दिखाता है कि &lt;see cref="Aspose.Tasks.Visualization.PageSettings" /&gt; के साथ कैसे काम किया जाए।

```csharp
var project = new Project(DataDir + "Project2.mpp");

// सेटिंग्स प्राप्त करें
var settings = project.DefaultView.PageInfo.PageSettings;
// कुछ गुणों को समायोजित करें
// पृष्ठ अभिविन्यास पोर्ट्रेट है या नहीं, यह दर्शाने वाला मान सेट करें; यदि पृष्ठ अभिविन्यास लैंडस्केप है तो false लौटाता है।
settings.IsPortrait = true;
// प्रिंट किए जाने वाले चौड़ाई में पृष्ठों की संख्या सेट करें।
settings.PagesInWidth = 5;
// प्रिंट किए जाने वाले ऊँचाई में पृष्ठों की संख्या सेट करें।
settings.PagesInHeight = 7;
// प्रिंटिंग को समायोजित करने के लिए सामान्य आकार का प्रतिशत सेट करें।
settings.PercentOfNormalSize = 200;
// कागज़ का आकार सेट करें। यह <see cref="T:Aspose.Tasks.Visualization.PrinterPaperSize" /> enumeration के मानों में से एक हो सकता है।
settings.PaperSize = PrinterPaperSize.PaperB4;
// प्रिंटिंग के लिए पहला पृष्ठ संख्या सेट करें।
settings.FirstPageNumber = 3;

SimpleSaveOptions options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "TestCanWritePageSettings.mpp", options);
```

### संबंधित देखें

* enum [PrinterPaperSize](../../printerpapersize/)
* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


