---
title: "TextStyle.ItemType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TextStyle प्रॉपर्टी। टेक्स्ट स्टाइल का TextItemType प्राप्त करता है या सेट करता है"
type: docs
weight: 60
url: /hi/net/aspose.tasks.visualization/textstyle/itemtype/
---
## TextStyle.ItemType property

टेक्स्ट स्टाइल का [`TextItemType`](../../textitemtype/) प्राप्त करता है या सेट करता है।

```csharp
public virtual TextItemType ItemType { get; set; }
```

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

* enum [TextItemType](../../textitemtype/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


