---
title: "SaveOptions.TextStyles"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveOptions प्रॉपर्टी। प्रोजेक्ट व्यू के रेंडरिंग के दौरान लागू होने वाले टेक्स्ट स्टाइल्स की सूची प्राप्त करता है या सेट करता है।"
type: docs
weight: 190
url: /hi/net/aspose.tasks.saving/saveoptions/textstyles/
---
## SaveOptions.TextStyles property

प्रोजेक्ट व्यू के रेंडरिंग के दौरान लागू होने वाले टेक्स्ट शैलियों की सूची को प्राप्त करता है या सेट करता है।

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## टिप्पणियाँ

ये स्टाइल्स GanttCharView.TextStyles में परिभाषित स्टाइल्स को ओवरराइड करते हैं।

## उदाहरण

दिखाता है कि कैसे सहेज विकल्पों के टेक्स्ट स्टाइल्स का उपयोग किया जाए जो प्रोजेक्ट में विभिन्न टेक्स्ट आइटम्स को स्टाइल करने के लिए उपयोग होते हैं।

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle(FontStyles.Bold | FontStyles.Italic)
{
    Color = Color.OrangeRed
};

style.ItemType = TextItemType.OverallocatedResources;

options.TextStyles = new List<TextStyle>
{
    style
};

project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### संबंधित देखें

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


