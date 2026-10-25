---
title: "क्लास PageLegend"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.PageLegend क्लास। एक पेज लेजेंड का प्रतिनिधित्व करता है जो प्रोजेक्ट प्रिंटिंग के लिए उपयोग किया जाता है।"
type: docs
weight: 3210
url: /hi/net/aspose.tasks.visualization/pagelegend/
---
## PageLegend class

प्रोजेक्ट प्रिंटिंग के लिए उपयोग किए जाने वाले पेज लेजेंड को दर्शाता है।

```csharp
public class PageLegend : HeaderFooterInfo
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [PageLegend](pagelegend/)() | डिफ़ॉल्ट कन्स्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | पैरेंट एलिमेंट में प्रदर्शित होने वाली केंद्रित इमेज को प्राप्त करता है या सेट करता है। |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | केंद्र इमेज के प्रदर्शित आकार को प्राप्त करता है या सेट करता है। |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | पैरेंट एलिमेंट में प्रदर्शित होने वाले केंद्रित टेक्स्ट को प्राप्त करता है या सेट करता है। |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | पैरेंट एलिमेंट में प्रदर्शित होने वाली बाएँ संरेखित छवि को प्राप्त करता है या सेट करता है। |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | बाएँ छवि के प्रदर्शित आकार को प्राप्त करता है या सेट करता है। |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | पैरेंट एलिमेंट में प्रदर्शित करने के लिए बाएँ संरेखित पाठ को प्राप्त करता है या सेट करता है। |
| [LegendOn](../../aspose.tasks.visualization/pagelegend/legendon/) { get; set; } | लेजेंड जहाँ दिखाई देता है, उन पेजों को प्राप्त करता है या सेट करता है। यह [`Legend`](../legend/) एनेमरेशन के मानों में से एक हो सकता है। |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | पैरेंट एलिमेंट में प्रदर्शित होने वाली दाएँ संरेखित छवि को प्राप्त करता है या सेट करता है। |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | दाएँ छवि के प्रदर्शित आकार को प्राप्त करता है या सेट करता है। |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | पैरेंट एलिमेंट में प्रदर्शित करने के लिए दाएँ संरेखित पाठ को प्राप्त करता है या सेट करता है। |
| [Width](../../aspose.tasks.visualization/pagelegend/width/) { get; set; } | लेजेंड के बाएँ भाग (डिफ़ॉल्ट रूप से प्रोजेक्ट का नाम और तिथि शामिल) की चौड़ाई सेंटीमीटर में प्राप्त करता है या सेट करता है। |

## उदाहरण

पेज लेजेंड जानकारी के साथ काम करने का तरीका दर्शाता है।

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// पेज लेजेंड जानकारी पढ़ें
var legend = project.DefaultView.PageInfo.Legend;

Console.WriteLine("Legend left text: {0} ", legend.LeftText);
Console.WriteLine("Legend left image: {0} ", legend.LeftImage);
Console.WriteLine("Legend center text: {0} ", legend.CenteredText);
Console.WriteLine("Legend center image: {0} ", legend.CenteredImage);
Console.WriteLine("Legend right text: {0} ", legend.RightText);
Console.WriteLine("Legend right image: {0} ", legend.RightImage);
Console.WriteLine("Legend On: {0} ", legend.LegendOn);
Console.WriteLine("Legend Width: {0} ", legend.Width);

// लेजेंड का संशोधन भी समर्थित है
legend.LeftText = "New Left Text";

project.Save(OutDir + "WorkWithPageLegend_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* class [HeaderFooterInfo](../headerfooterinfo/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


