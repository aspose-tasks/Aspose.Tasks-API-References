---
title: "TextStyle.BackgroundPattern"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية TextStyle. يحصل أو يضبط نمط الخلفية لنمط النص. BackgroundPattern"
type: docs
weight: 30
url: /ar/net/aspose.tasks.visualization/textstyle/backgroundpattern/
---
## TextStyle.BackgroundPattern property

يحصل أو يعيّن نمط الخلفية لنمط النص. `BackgroundPattern`.

```csharp
public BackgroundPattern BackgroundPattern { get; set; }
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

* enum [BackgroundPattern](../../../aspose.tasks/backgroundpattern/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


