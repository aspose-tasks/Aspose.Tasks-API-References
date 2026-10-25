---
title: "TextStyle.Font"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية TextStyle. يحصل أو يعيّن الخط لنمط النص"
type: docs
weight: 50
url: /ar/net/aspose.tasks.visualization/textstyle/font/
---
## TextStyle.Font property

يحصل أو يعيّن خط نمط النص.

```csharp
public FontDescriptor Font { get; set; }
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

* class [FontDescriptor](../../fontdescriptor/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


