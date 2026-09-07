---
title: "क्लास TextStyle"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.TextStyle क्लास। प्रोजेक्ट व्यू में किसी आइटम के लिए टेक्स्ट की दृश्य शैली बदलें"
type: docs
weight: 3420
url: /hi/net/aspose.tasks.visualization/textstyle/
---
## TextStyle class

प्रोजेक्ट दृश्य में आइटम के लिए टेक्स्ट की दृश्य शैली बदलें।

```csharp
public class TextStyle
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [TextStyle](textstyle/#constructor)() | `TextStyle` क्लास का नया इंस्टेंस डिफ़ॉल्ट सेटिंग्स के साथ इनिशियलाइज़ करता है। |
| [TextStyle](textstyle/#constructor_1)(FontDescriptor) | `TextStyle` क्लास का नया इंस्टेंस निर्दिष्ट फ़ॉन्ट सेटिंग्स के साथ इनिशियलाइज़ करता है। |
| [TextStyle](textstyle/#constructor_2)(FontStyles) | `TextStyle` क्लास का नया इंस्टेंस डिफ़ॉल्ट फ़ॉन्ट और निर्दिष्ट फ़ॉन्ट शैली के साथ इनिशियलाइज़ करता है। |
| [TextStyle](textstyle/#constructor_3)(float, FontStyles) | `TextStyle` क्लास का नया इंस्टेंस डिफ़ॉल्ट फ़ॉन्ट और निर्दिष्ट फ़ॉन्ट आकार एवं शैली के साथ इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | टेक्स्ट शैली का बैकग्राउंड रंग प्राप्त करता है या सेट करता है। [`Color`](./color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | टेक्स्ट शैली का बैकग्राउंड पैटर्न प्राप्त करता है या सेट करता है। [`BackgroundPattern`](./backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | टेक्स्ट का रंग प्राप्त करता है या सेट करता है। |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | टेक्स्ट शैली का फ़ॉन्ट प्राप्त करता है या सेट करता है। |
| virtual [ItemType](../../aspose.tasks.visualization/textstyle/itemtype/) { get; set; } | टेक्स्ट शैली का [`TextItemType`](../textitemtype/) प्राप्त करता है या सेट करता है। |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


