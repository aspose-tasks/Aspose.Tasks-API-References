---
title: "تعداد BackgroundPattern"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.BackgroundPattern. يحدد نمط الخلفية"
type: docs
weight: 100
url: /ar/net/aspose.tasks/backgroundpattern/
---
## BackgroundPattern enumeration

يحدد نمط الخلفية.

```csharp
public enum BackgroundPattern
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| DarkDiagonalLeft | `7` | يشير إلى نمط خلفية قطري أيسر داكن. |
| DarkDiagonalRight | `8` | يشير إلى نمط خلفية قطري أيمن داكن. |
| DarkDither | `13` | يشير إلى نمط خلفية تمويه داكن. |
| DarkFill | `4` | يشير إلى نمط خلفية تعبئة داكن. |
| DiagonalLeft | `5` | يشير إلى نمط خلفية مائل إلى اليسار. |
| DiagonalRight | `6` | يشير إلى نمط خلفية مائل إلى اليمين. |
| Hollow | `0` | يشير إلى نمط خلفية مجوف. |
| LightDither | `11` | يشير إلى نمط خلفية تمويه خفيف. |
| LightFill | `2` | يشير إلى نمط خلفية تعبئة خفيفة. |
| MediumDither | `12` | يشير إلى نمط خلفية تمويه متوسط. |
| MediumFill | `3` | يشير إلى نمط خلفية تعبئة متوسطة. |
| MediumVerticalStripe | `10` | يشير إلى نمط خلفية خطوط عمودية متوسطة. |
| SolidFill | `1` | يشير إلى نمط خلفية تعبئة صلبة. |
| ThinVerticalStripe | `9` | يشير إلى نمط خلفية خطوط عمودية رقيقة. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


