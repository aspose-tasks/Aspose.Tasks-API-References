---
title: "क्लास HeaderFooterInfo"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.HeaderFooterInfo क्लास। हेडर फुटर या लेजेंड की विज़ुअल सामग्री का प्रतिनिधित्व करता है जो व्यूज़ के प्रिंटिंग और रेंडरिंग के लिए उपयोग होती है।"
type: docs
weight: 3130
url: /hi/net/aspose.tasks.visualization/headerfooterinfo/
---
## HeaderFooterInfo class

हेडर, फुटर या लेजेंड की दृश्य सामग्री को दर्शाता है जिसका उपयोग दृश्यों के प्रिंटिंग/रेंडरिंग के लिए किया जाता है।

```csharp
public class HeaderFooterInfo
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [HeaderFooterInfo](headerfooterinfo/)() | `HeaderFooterInfo` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | पैरेंट एलिमेंट में प्रदर्शित होने वाली केंद्रित इमेज को प्राप्त करता है या सेट करता है। |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | केंद्र इमेज के प्रदर्शित आकार को प्राप्त करता है या सेट करता है। |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | पैरेंट एलिमेंट में प्रदर्शित होने वाले केंद्रित टेक्स्ट को प्राप्त करता है या सेट करता है। |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | पैरेंट एलिमेंट में प्रदर्शित होने वाली बाएँ संरेखित छवि को प्राप्त करता है या सेट करता है। |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | बाएँ छवि के प्रदर्शित आकार को प्राप्त करता है या सेट करता है। |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | पैरेंट एलिमेंट में प्रदर्शित करने के लिए बाएँ संरेखित पाठ को प्राप्त करता है या सेट करता है। |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | पैरेंट एलिमेंट में प्रदर्शित होने वाली दाएँ संरेखित छवि को प्राप्त करता है या सेट करता है। |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | दाएँ छवि के प्रदर्शित आकार को प्राप्त करता है या सेट करता है। |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | पैरेंट एलिमेंट में प्रदर्शित करने के लिए दाएँ संरेखित पाठ को प्राप्त करता है या सेट करता है। |

## उदाहरण

पृष्ठ हेडर/फ़ूटर जानकारी को कैसे पढ़ें, यह दिखाता है।

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var info = project.DefaultView.PageInfo;

Console.WriteLine("Header left text: {0} ", info.Header.LeftText);
Console.WriteLine("Header left image: {0} ", info.Header.LeftImage);
Console.WriteLine("Header left image size: {0} ", info.Header.LeftImageSize);
Console.WriteLine("Header center text: {0} ", info.Header.CenteredText);
Console.WriteLine("Header center image: {0} ", info.Header.CenteredImage);
Console.WriteLine("Header center image size: {0} ", info.Header.CenteredImageSize);
Console.WriteLine("Header right text: {0} ", info.Header.RightText);
Console.WriteLine("Header right image: {0} ", info.Header.RightImage);
Console.WriteLine("Header right image size: {0} ", info.Header.RightImageSize);
Console.WriteLine();
Console.WriteLine("Footer left text: {0} ", info.Footer.LeftText);
Console.WriteLine("Footer left image: {0} ", info.Footer.LeftImage);
Console.WriteLine("Footer left image size: {0} ", info.Footer.LeftImageSize);
Console.WriteLine("Footer center text: {0} ", info.Footer.CenteredText);
Console.WriteLine("Footer center image: {0} ", info.Footer.CenteredImage);
Console.WriteLine("Footer center size: {0} ", info.Footer.CenteredImageSize);
Console.WriteLine("Footer right text: {0} ", info.Footer.RightText);
Console.WriteLine("Footer right image: {0} ", info.Footer.RightImage);
Console.WriteLine("Footer right image size: {0} ", info.Footer.RightImageSize);
```

### संबंधित देखें

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


