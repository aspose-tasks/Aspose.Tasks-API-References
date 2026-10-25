---
title: "SaveOptions.TextStyles"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SaveOptions. تحصل أو تعين قائمة أنماط النص التي تُطبق أثناء تصوير عرض المشروع"
type: docs
weight: 190
url: /ar/net/aspose.tasks.saving/saveoptions/textstyles/
---
## SaveOptions.TextStyles property

يحصل أو يعيّن قائمة أنماط النص التي تُطبق أثناء عرض منظور المشروع.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## ملاحظات

هذه الأنماط تتجاوز الأنماط المعرفة في GanttCharView.TextStyles.

## الأمثلة

يوضح كيفية استخدام أنماط النص في خيارات الحفظ التي تُستخدم لتنسيق عناصر **text** المختلفة في مشروع.

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

### انظر أيضًا

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


