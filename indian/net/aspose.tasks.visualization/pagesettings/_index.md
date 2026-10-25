---
title: "क्लास PageSettings"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.PageSettings क्लास। प्रोजेक्ट व्यू के एक पृष्ठ के प्रिंट सेटिंग्स को दर्शाता है।"
type: docs
weight: 3240
url: /hi/net/aspose.tasks.visualization/pagesettings/
---
## PageSettings class

प्रोजेक्ट दृश्य के एक पेज के लिए प्रिंटिंग सेटिंग्स को दर्शाता है।

```csharp
public class PageSettings
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [PageSettings](pagesettings/)() | `PageSettings` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। प्रोजेक्ट व्यू के एक पृष्ठ के प्रिंट सेटिंग्स को दर्शाता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [AdjustToPercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/) { get; set; } | प्रिंटिंग को सामान्य आकार के निर्दिष्ट प्रतिशत ([`PercentOfNormalSize`](./percentofnormalsize/)) तक समायोजित करने के लिए मान प्राप्त करता है या सेट करता है। |
| [FirstPageNumber](../../aspose.tasks.visualization/pagesettings/firstpagenumber/) { get; set; } | प्रिंटिंग के लिए पहला पृष्ठ संख्या प्राप्त करता है या सेट करता है। |
| [IsPortrait](../../aspose.tasks.visualization/pagesettings/isportrait/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि पेज अभिविन्यास पोर्ट्रेट है; यदि पेज अभिविन्यास लैंडस्केप है तो false लौटाता है। |
| [PagesInHeight](../../aspose.tasks.visualization/pagesettings/pagesinheight/) { get; set; } | प्रिंट किए जाने वाले ऊँचाई में पृष्ठों की संख्या प्राप्त करता है या सेट करता है। |
| [PagesInWidth](../../aspose.tasks.visualization/pagesettings/pagesinwidth/) { get; set; } | प्रिंट किए जाने वाले चौड़ाई में पृष्ठों की संख्या प्राप्त करता है या सेट करता है। |
| [PaperSize](../../aspose.tasks.visualization/pagesettings/papersize/) { get; set; } | कागज़ का आकार प्राप्त करता है या सेट करता है। यह [`PrinterPaperSize`](../printerpapersize/) enumeration के मानों में से एक हो सकता है। |
| [PaperSizeId](../../aspose.tasks.visualization/pagesettings/papersizeid/) { get; set; } | PrinterPaperSize मानों में से एक या कस्टम पेज आकार आईडी का प्रतिनिधित्व करने वाला पूर्णांक प्राप्त करता है या सेट करता है। इस मान का उपयोग OS सेटिंग्स से PaperSize प्राप्त करने के लिए किया जा सकता है। |
| [PercentOfNormalSize](../../aspose.tasks.visualization/pagesettings/percentofnormalsize/) { get; set; } | प्रिंटिंग को समायोजित करने के लिए सामान्य आकार का प्रतिशत प्राप्त करता है या सेट करता है। |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


