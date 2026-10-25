---
title: "TextStyle.ItemType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية TextStyle. يحصل أو يضبط TextItemType لنمط النص"
type: docs
weight: 60
url: /ar/net/aspose.tasks.visualization/textstyle/itemtype/
---
## TextStyle.ItemType property

يحصل أو يضبط [`TextItemType`](../../textitemtype/) لنمط النص.

```csharp
public virtual TextItemType ItemType { get; set; }
```

## الأمثلة

يوضح كيفية تخصيص أنماط النص التي تُستخدم لتنسيق عناصر النص المختلفة في المشروع.

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

### انظر أيضًا

* enum [TextItemType](../../textitemtype/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


