---
title: "HeaderFooterInfo.RightText"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "HeaderFooterInfo प्रॉपर्टी। दाएँ संरेखित टेक्स्ट को प्राप्त करता है या सेट करता है जिसे पैरेंट एलिमेंट में प्रदर्शित किया जाता है"
type: docs
weight: 100
url: /hi/net/aspose.tasks.visualization/headerfooterinfo/righttext/
---
## HeaderFooterInfo.RightText property

पैरेंट एलिमेंट में प्रदर्शित करने के लिए दाएँ संरेखित पाठ को प्राप्त करता है या सेट करता है।

```csharp
public string RightText { get; set; }
```

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

* class [HeaderFooterInfo](../)
* namespace [Aspose.Tasks.Visualization](../../headerfooterinfo/)
* assembly [Aspose.Tasks](../../../)


