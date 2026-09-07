---
title: "PageInfo.Legend"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PageInfo प्रॉपर्टी। PageLegend क्लास का एक इंस्टेंस प्राप्त करता है या सेट करता है जो पेज लेजेंड के रेंडरिंग विकल्पों को निर्दिष्ट करता है"
type: docs
weight: 40
url: /hi/net/aspose.tasks.visualization/pageinfo/legend/
---
## PageInfo.Legend property

[`PageLegend`](../../pagelegend/) क्लास का एक इंस्टेंस प्राप्त करता है या सेट करता है जो पेज लेजेंड के रेंडरिंग विकल्पों को निर्दिष्ट करता है।

```csharp
public PageLegend Legend { get; set; }
```

## टिप्पणियाँ

वर्तमान में यह केवल Gantt Chart व्यूज़ पर लागू है।

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

* class [PageLegend](../../pagelegend/)
* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


