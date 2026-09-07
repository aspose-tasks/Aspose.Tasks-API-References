---
title: "क्लास PageInfo"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.PageInfo क्लास। पेज सेटअप डेटा का प्रतिनिधित्व करता है जो MPP फ़ाइल फ़ॉर्मेट में मौजूद है और प्रिंटिंग के लिए उपयोग किया जाता है।"
type: docs
weight: 3200
url: /hi/net/aspose.tasks.visualization/pageinfo/
---
## PageInfo class

MPP फ़ाइल प्रारूप में मौजूद पेज सेटअप डेटा को दर्शाता है और प्रिंटिंग के लिए उपयोग किया जाता है।

```csharp
public class PageInfo
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [PageInfo](pageinfo/)() | `PageInfo` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। पेज सेटअप डेटा का प्रतिनिधित्व करता है जो MPP फ़ाइल फ़ॉर्मेट में मौजूद है और प्रिंटिंग के लिए उपयोग किया जाता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Footer](../../aspose.tasks.visualization/pageinfo/footer/) { get; set; } | [`HeaderFooterInfo`](../headerfooterinfo/) क्लास का एक इंस्टेंस प्राप्त करता है या सेट करता है जो फुटर डेटा का प्रतिनिधित्व करता है। |
| [Header](../../aspose.tasks.visualization/pageinfo/header/) { get; set; } | [`HeaderFooterInfo`](../headerfooterinfo/) क्लास का इंस्टेंस प्राप्त करता है या सेट करता है जो हेडर डेटा का प्रतिनिधित्व करता है। |
| [Legend](../../aspose.tasks.visualization/pageinfo/legend/) { get; set; } | [`PageLegend`](../pagelegend/) क्लास का एक इंस्टेंस प्राप्त करता है या सेट करता है जो पेज लेजेंड के रेंडरिंग विकल्प निर्दिष्ट करता है। |
| [Margins](../../aspose.tasks.visualization/pageinfo/margins/) { get; } | [`PageMargins`](../pagemargins/) क्लास का एक इंस्टेंस प्राप्त करता है जो पेज मार्जिन निर्दिष्ट करता है। |
| [Name](../../aspose.tasks.visualization/pageinfo/name/) { get; } | जिस व्यू के लिए सेट‑अप डेटा उपयोग किया जाता है, उसका नाम प्राप्त करता है। |
| [PageSettings](../../aspose.tasks.visualization/pageinfo/pagesettings/) { get; } | [`PageSettings`](./pagesettings/) क्लास का एक इंस्टेंस प्राप्त करता है जो पेज प्रिंटिंग सेटिंग्स निर्दिष्ट करता है। |
| [PageViewSettings](../../aspose.tasks.visualization/pageinfo/pageviewsettings/) { get; } | [`PageViewSettings`](./pageviewsettings/) क्लास का एक इंस्टेंस प्राप्त करता है जो पेज व्यू प्रिंटिंग सेटिंग्स निर्दिष्ट करता है। |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


