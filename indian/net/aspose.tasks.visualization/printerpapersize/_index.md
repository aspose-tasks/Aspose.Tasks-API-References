---
title: "एनम PrinterPaperSize"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.PrinterPaperSize एनम। प्रिंटिंग के लिए उपयोग किए जाने वाले पेपर साइज को निर्दिष्ट करता है"
type: docs
weight: 3280
url: /hi/net/aspose.tasks.visualization/printerpapersize/
---
## PrinterPaperSize enumeration

प्रिंटिंग के लिए उपयोग किए जाने वाले कागज़ के आकार को निर्दिष्ट करता है।

```csharp
public enum PrinterPaperSize
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Custom | `1` | इसे दर्शाता है कि पेपर साइज उपयोगकर्ता द्वारा परिभाषित है। |
| PaperLetter | `1` | संकेत करता है लिफ़ाफ़ा लेटर प्रिंटर कागज़ आकार (8.5 in. by 11 in.). |
| PaperLetterSmall | `2` | संकेत करता है छोटा लेटर प्रिंटर कागज़ आकार (8.5 in. by 11 in.). |
| PaperTabloid | `3` | संकेत करता है टैब्लॉइड प्रिंटर कागज़ आकार (11 in. by 17 in.). |
| PaperLedger | `4` | संकेत करता है लेजर प्रिंटर कागज़ आकार (17 in. by 11 in.). |
| PaperLegal | `5` | संकेत करता है लिफ़ाफ़ा लीगल प्रिंटर कागज़ आकार (8.5 in. by 14 in.). |
| PaperStatement | `6` | संकेत करता है स्टेटमेंट प्रिंटर कागज़ आकार (5.5 in. by 8.5 in.). |
| PaperExecutive | `7` | संकेत करता है लिफ़ाफ़ा एग्जीक्यूटिव प्रिंटर कागज़ आकार (7.25 in. by 10.5 in.). |
| PaperA3 | `8` | संकेत करता है A3 प्रिंटर कागज़ आकार (297 mm by 420 mm). |
| PaperA4 | `9` | संकेत करता है A4 प्रिंटर कागज़ आकार (210 mm by 297 mm). |
| PaperA4Small | `10` | संकेत करता है छोटा A4 प्रिंटर कागज़ आकार (210 mm by 297 mm). |
| PaperA5 | `11` | संकेत करता है A5 प्रिंटर कागज़ आकार (148 mm by 210 mm). |
| PaperB4 | `12` | संकेत करता है B4 प्रिंटर कागज़ आकार (250 mm by 353 mm). |
| PaperB5 | `13` | संकेत करता है B5 प्रिंटर कागज़ आकार (176 mm by 250 mm). |
| PaperFolio | `14` | संकेत करता है फ़ोलियो प्रिंटर कागज़ आकार (8.5 in. by 13 in.). |
| PaperQuarto | `15` | संकेत करता है क्वार्टो प्रिंटर कागज़ आकार (215 mm by 275 mm). |
| PaperStandard10x14 | `16` | संकेत करता है स्टैंडर्ड प्रिंटर कागज़ आकार (10 in. by 14 in.). |
| PaperStandard11x17 | `17` | संकेत करता है स्टैंडर्ड प्रिंटर कागज़ आकार (11 in. by 17 in.). |
| PaperNote | `18` | संकेत करता है नोट प्रिंटर कागज़ आकार (8.5 in. by 11 in.). |
| PaperEnvelope10 | `20` | संकेत करता है लिफ़ाफ़ा10 प्रिंटर कागज़ आकार (4.125 in. by 9.5 in.). |
| PaperCSheet | `24` | संकेत करता है C पेपर प्रिंटर कागज़ आकार (17 in. by 22 in.). |
| PaperDSheet | `25` | संकेत करता है D पेपर प्रिंटर कागज़ आकार (22 in. by 34 in.). |
| PaperESheet | `26` | संकेत करता है E पेपर प्रिंटर कागज़ आकार (34 in. by 44 in.). |
| PaperEnvelopeMonarch | `37` | संकेत करता है लिफ़ाफ़ा मोनार्क प्रिंटर कागज़ आकार (3.875 in. by 7.5 in.). |
| PaperStandard9x11 | `44` | संकेत करता है स्टैंडर्ड प्रिंटर कागज़ आकार (9 in. by 11 in.). |
| PaperStandard10x11 | `45` | संकेत करता है स्टैंडर्ड प्रिंटर कागज़ आकार (10 in. by 11 in.). |
| PaperStandard15x11 | `46` | मानक प्रिंटर कागज़ का आकार दर्शाता है (15 इंच बाय 11 इंच)। |
| PaperA2 | `66` | A2 प्रिंटर कागज़ का आकार दर्शाता है (420 मिमी बाय 594 मिमी)। |

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


