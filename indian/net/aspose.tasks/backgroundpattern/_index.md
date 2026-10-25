---
title: "एन्यूम BackgroundPattern"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.BackgroundPattern enum. बैकग्राउंड पैटर्न निर्दिष्ट करता है"
type: docs
weight: 100
url: /hi/net/aspose.tasks/backgroundpattern/
---
## BackgroundPattern enumeration

पृष्ठभूमि पैटर्न को निर्दिष्ट करता है।

```csharp
public enum BackgroundPattern
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| DarkDiagonalLeft | `7` | डार्क डायगोनल लेफ्ट बैकग्राउंड पैटर्न दर्शाता है। |
| DarkDiagonalRight | `8` | डार्क डायगोनल राइट बैकग्राउंड पैटर्न दर्शाता है। |
| DarkDither | `13` | डार्क डिथर बैकग्राउंड पैटर्न दर्शाता है। |
| DarkFill | `4` | डार्क फिल बैकग्राउंड पैटर्न दर्शाता है। |
| DiagonalLeft | `5` | डायगोनल बाएँ पृष्ठभूमि पैटर्न को दर्शाता है। |
| DiagonalRight | `6` | डायगोनल दाएँ पृष्ठभूमि पैटर्न को दर्शाता है। |
| Hollow | `0` | होलो पृष्ठभूमि पैटर्न को दर्शाता है। |
| LightDither | `11` | हल्का डिथर पृष्ठभूमि पैटर्न को दर्शाता है। |
| LightFill | `2` | हल्का भराव पृष्ठभूमि पैटर्न को दर्शाता है। |
| MediumDither | `12` | मध्यम डिथर पृष्ठभूमि पैटर्न को दर्शाता है। |
| MediumFill | `3` | मध्यम भराव पृष्ठभूमि पैटर्न को दर्शाता है। |
| MediumVerticalStripe | `10` | मध्यम ऊर्ध्वाधर धारी पृष्ठभूमि पैटर्न को दर्शाता है। |
| SolidFill | `1` | सॉलिड भराव पृष्ठभूमि पैटर्न को दर्शाता है। |
| ThinVerticalStripe | `9` | पतली ऊर्ध्वाधर धारी पृष्ठभूमि पैटर्न को दर्शाता है। |

## उदाहरण

दिखाता है कि प्रोजेक्ट में विभिन्न टेक्स्ट आइटम्स को स्टाइल करने के लिए उपयोग किए जाने वाले टेक्स्ट स्टाइल्स को कैसे कस्टमाइज़ किया जाए।

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle();
style.Color = Color.OrangeRed;
style.Font = new FontDescriptor(FontFamily.GenericMonospace.Name, 10F, FontStyles.Bold | FontStyles.Italic);
style.ItemType = TextItemType.OverallocatedResources;
style.BackgroundColor = Color.Aqua;
style.BackgroundPattern = BackgroundPattern.DarkDither;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


