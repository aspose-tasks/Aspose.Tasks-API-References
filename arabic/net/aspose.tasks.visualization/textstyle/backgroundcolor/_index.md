---
title: "TextStyle.BackgroundColor"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية TextStyle. يحصل أو يضبط لون الخلفية لنمط النص. Color"
type: docs
weight: 20
url: /ar/net/aspose.tasks.visualization/textstyle/backgroundcolor/
---
## TextStyle.BackgroundColor property

يحصل أو يضبط لون الخلفية لنمط النص. [`Color`](../color/).

```csharp
public Color BackgroundColor { get; set; }
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

* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


