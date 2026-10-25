---
title: "PageInfo.PageInfo"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PageInfo कंस्ट्रक्टर। PageInfo क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। यह पेज सेटअप डेटा का प्रतिनिधित्व करता है जो MPP फ़ाइल फ़ॉर्मेट में मौजूद है और प्रिंटिंग के लिए उपयोग किया जाता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks.visualization/pageinfo/pageinfo/
---
## PageInfo constructor

[`PageInfo`](../) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। यह पेज सेटअप डेटा का प्रतिनिधित्व करता है जो MPP फ़ाइल फ़ॉर्मेट में मौजूद है और प्रिंटिंग के लिए उपयोग किया जाता है।

```csharp
public PageInfo()
```

## उदाहरण

MS Project व्यू के पेज इन्फो के साथ काम करने का तरीका दर्शाता है।

```csharp
var project = new Project(DataDir + "Project2.mpp");

// डिफ़ॉल्ट व्यू को संशोधित करने देता है
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// मार्जिन को संशोधित करने देता है
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// पेज सेटिंग्स को संशोधित करें
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// पेज व्यू सेटिंग्स को संशोधित करें
// नोट्स को प्रिंट करने का संकेत देने वाला मान सेट करें।
info.PageViewSettings.PrintNotes = true;

var header = new HeaderFooterInfo
{
    LeftText = "Left header text",
    CenteredText = "Centered header text",
    RightText = "Right header text"
};
var legend = new PageLegend
{
    LeftText =  "Left legend text",
    CenteredText = "Centered legend text",
    RightText = "Right legend text"
};
var footer = new HeaderFooterInfo
{
    LeftText = "Left footer text",
    CenteredText = "Centered footer text",
    RightText = "Right footer text"
};

info.Header = header;
info.Legend = legend;
info.Footer = footer;

// परियोजना के साथ काम करें...
```

### संबंधित देखें

* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


