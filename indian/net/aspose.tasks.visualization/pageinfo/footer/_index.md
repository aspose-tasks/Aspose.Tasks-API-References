---
title: "PageInfo.Footer"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PageInfo प्रॉपर्टी। HeaderFooterInfo क्लास का एक उदाहरण प्राप्त करता है या सेट करता है जो फुटर डेटा का प्रतिनिधित्व करता है"
type: docs
weight: 20
url: /hi/net/aspose.tasks.visualization/pageinfo/footer/
---
## PageInfo.Footer property

[`HeaderFooterInfo`](../../headerfooterinfo/) क्लास का एक उदाहरण प्राप्त करता है या सेट करता है जो फुटर डेटा का प्रतिनिधित्व करता है।

```csharp
public HeaderFooterInfo Footer { get; set; }
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

* class [HeaderFooterInfo](../../headerfooterinfo/)
* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


