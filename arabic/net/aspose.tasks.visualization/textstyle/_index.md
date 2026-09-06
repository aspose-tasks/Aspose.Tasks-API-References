---
title: "الفئة TextStyle"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Visualization.TextStyle. غيّر النمط البصري للنص لعنصر في عرض المشروع"
type: docs
weight: 3420
url: /ar/net/aspose.tasks.visualization/textstyle/
---
## TextStyle class

غيّر النمط البصري للنص للعنصر في عرض المشروع.

```csharp
public class TextStyle
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [TextStyle](textstyle/#constructor)() | ينشئ مثيلاً جديدًا من الفئة `TextStyle` بالإعدادات الافتراضية. |
| [TextStyle](textstyle/#constructor_1)(FontDescriptor) | ينشئ مثيلاً جديدًا من الفئة `TextStyle` بإعدادات الخط المحددة. |
| [TextStyle](textstyle/#constructor_2)(FontStyles) | ينشئ مثيلاً جديدًا من الفئة `TextStyle` بالخط الافتراضي والنمط المحدد للخط. |
| [TextStyle](textstyle/#constructor_3)(float, FontStyles) | ينشئ مثيلاً جديدًا من الفئة `TextStyle` بالخط الافتراضي وحجم الخط والنمط المحددين. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | يحصل أو يعيّن لون الخلفية لنمط النص. [`Color`](./color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | يحصل أو يعيّن نمط الخلفية لنمط النص. [`BackgroundPattern`](./backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | يحصل أو يعيّن لون النص. |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | يحصل أو يعيّن خط نمط النص. |
| virtual [ItemType](../../aspose.tasks.visualization/textstyle/itemtype/) { get; set; } | يحصل أو يعيّن [`TextItemType`](../textitemtype/) لنمط النص. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


